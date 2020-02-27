## About Laravel-base

Terimaksih kepada Allah SWT.
Aplikasi ini dibuat untuk mempermudah pembuatan aplikasi, dengan menghadirkan fitur roles dan permission, app setting, user management.
dan telah terinstall admin template.

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

## How To Install

# 1
Clone Repository
-git clone https://github.com/FarhanRiuzaki/laravel-base.git
-cp .env.example .env

# 2
Open .ENV
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=database_name
DB_USERNAME=root
DB_PASSWORD=password

# 3
Database
-create database

# 4
Artisan
-php artisan migrate

# 5
RUN IN SQL
/*
 Navicat Premium Data Transfer

 Source Server         : LOCALHOST
 Source Server Type    : MySQL
 Source Server Version : 50729
 Source Host           : localhost:3306
 Source Schema         : laravel_base

 Target Server Type    : MySQL
 Target Server Version : 50729
 File Encoding         : 65001

 Date: 14/02/2020 11:05:52
*/

SET NAMES utf8mb4;
SET FOREIGN_KEY_CHECKS = 0;


-- ----------------------------
-- Records of model_has_roles
-- ----------------------------
BEGIN;
INSERT INTO `model_has_roles` VALUES (1, 'App\\User', 2);
INSERT INTO `model_has_roles` VALUES (99, 'App\\User', 5);
COMMIT;


-- ----------------------------
-- Records of permissions
-- ----------------------------
BEGIN;
INSERT INTO `permissions` VALUES (1, 'apps-show', 'web', '2020-02-11 14:38:29', '2020-02-11 14:38:29');
INSERT INTO `permissions` VALUES (2, 'role-show', 'web', '2020-02-11 14:38:39', '2020-02-11 14:38:39');
INSERT INTO `permissions` VALUES (3, 'role permission-show', 'web', '2020-02-11 14:38:50', '2020-02-11 14:38:50');
INSERT INTO `permissions` VALUES (4, 'users-show', 'web', '2020-02-11 14:38:59', '2020-02-11 14:38:59');
COMMIT;

-- ----------------------------
-- Records of role_has_permissions
-- ----------------------------
BEGIN;
INSERT INTO `role_has_permissions` VALUES (1, 1);
INSERT INTO `role_has_permissions` VALUES (2, 1);
INSERT INTO `role_has_permissions` VALUES (3, 1);
INSERT INTO `role_has_permissions` VALUES (4, 1);
INSERT INTO `role_has_permissions` VALUES (1, 99);
INSERT INTO `role_has_permissions` VALUES (2, 99);
INSERT INTO `role_has_permissions` VALUES (3, 99);
INSERT INTO `role_has_permissions` VALUES (4, 99);
COMMIT;

-- ----------------------------
-- Records of roles
-- ----------------------------
BEGIN;
INSERT INTO `roles` VALUES (1, 'Admin', 'web', '2020-02-11 09:51:38', '2020-02-11 09:51:38');
INSERT INTO `roles` VALUES (6, 'User', 'web', '2020-02-11 11:23:50', '2020-02-11 11:23:50');
INSERT INTO `roles` VALUES (99, 'super-admin', 'web', '2020-02-11 15:03:43', '2020-02-11 15:03:43');
COMMIT;

-- ----------------------------
-- Records of users
-- ----------------------------
BEGIN;
INSERT INTO `users` VALUES (2, 'Administrator', 'admin@email.com', NULL, '$2y$10$iT79gWz9IU7QuG/wxuhNteROMwb1s9o3yVZREWC.KbB5DOZNUVW8i', 1, NULL, '2020-02-11 11:51:29', '2020-02-11 11:51:29');
INSERT INTO `users` VALUES (5, 'Farhan Riuzaki', 'admin@gmail.com', NULL, '$2y$10$Jn7jqNPLzI2As3cBehD61ORDUYRUnNo2lQrBjiBDyLrZlUv3M0LaC', 1, NULL, '2020-02-11 13:24:40', '2020-02-11 13:24:40');
COMMIT;



## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [riuzakif@gmail.com](mailto:riuzakif@gmail.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
