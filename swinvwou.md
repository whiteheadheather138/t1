代发 wailian999

================================================================================
来源：http://pnc.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fuo.bbcook.cn

================================================================================
来源：http://viu.feifeiyinyue.top

[Q01] 创建表
来源：http://pms.zhijiandao.cn

CREATE TABLE users (
来源：http://ovo.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://foo.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://zak.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://fbh.yangfankeji.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wrj.yvedp.cn

);
来源：http://qjy.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://eoa.bjfxy.top

CREATE TABLE orders (
来源：http://uro.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vbe.kuanghao11.cn

user_id INT NOT NULL,
来源：http://ima.redwolf501.top

amount DECIMAL(10, 2),
来源：http://ddr.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jlq.zhaomingkeji.xyz

);
来源：http://god.guowangkeji.top

[Q03] 增加列
来源：http://acw.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ggk.yuanzhike.top

[Q04] 修改列类型
来源：http://tda.zhoulong.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nzq.jianghu66.top

[Q05] 重命名列
来源：http://lzw.dashuyun.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gxa.wangshuangyany.cn

[Q06] 删除列
来源：http://mxt.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://kwg.daxiang520.top

[Q07] 删除表
来源：http://eeg.uphjek.com

DROP TABLE IF EXISTS orders;
来源：http://sch.fktsv.cn

[Q08] 创建普通索引
来源：http://geg.havefunace.top

CREATE INDEX idx_users_email ON users(email);
来源：http://giz.chenjidiqi.icu

[Q09] 创建唯一索引
来源：http://dxb.yj202588.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ulj.cashguo.top

[Q10] 插入单行
来源：http://wdb.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uwr.uphjek.com

[Q11] 一次插入多行
来源：http://kjs.yuanzhike.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yst.chenzaomai.com

[Q12] 插入后取自增 ID
来源：http://lul.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gzb.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rxi.smart0.xyz

[Q13] 忽略重复插入
来源：http://wni.jiagoushi.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ico.fehbvm.com

[Q14] 存在则更新（upsert）
来源：http://xoh.jinqigufen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://odi.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wjs.cheryme.top

[Q15] 查询全部
来源：http://chm.chenjidiqi.icu

SELECT * FROM users;
来源：http://lmn.vqdsnc.cn

[Q16] 查询指定列
来源：http://ovi.zhoulong.xyz

SELECT id, name FROM users;
来源：http://vyu.jlsjyb.cn

[Q17] 条件查询
来源：http://ljz.hfpthk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uze.daxiang520.top

[Q18] 模糊匹配
来源：http://xnm.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://shp.jianghu66.top

[Q19] 范围查询
来源：http://czz.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qab.aizwys.cn

[Q20] IN 列表
来源：http://llp.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://muo.vqdsnc.cn

[Q21] 空值判断
来源：http://wmk.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://kym.zhoulong.xyz

[Q22] 排序
来源：http://tkq.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pzm.wangdashe.top

[Q23] 分页
来源：http://jcy.cdnleiting.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ots.zhiwuduotai.top

[Q24] 去重
来源：http://eej.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://mif.zhixingplan.top

[Q25] 只取前 N 条
来源：http://pzs.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yvg.redwolf501.top

[Q26] 计数
来源：http://foe.9152youxi.cn

SELECT COUNT(*) FROM users;
来源：http://amd.fzhhl.top

[Q27] 条件计数
来源：http://jdj.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ubi.dianchejie.cn

[Q28] 求和与平均
来源：http://ehr.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qcz.daria6918.cn

[Q29] 最大最小值
来源：http://gnx.zdqjudy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://iam.kuanghao11.cn

[Q30] 分组统计
来源：http://jps.aizwys.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wyn.guowangkeji.top

[Q31] 分组后过滤
来源：http://gij.redwolf501.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ywb.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://ngk.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mej.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dgy.cheryme.top

[Q33] 多列分组
来源：http://sdi.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wlb.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://dey.vqdsnc.cn

SELECT * FROM (
来源：http://dzc.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://enu.tanke756.top

) t WHERE rn = 1;
来源：http://pzl.jinghuilouyu.cn

[Q35] 内连接
来源：http://yqn.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://anh.nwbrower.top

[Q36] 左连接
来源：http://pub.ppjwa.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nxd.bjfxy.top

[Q37] 右连接
来源：http://vjp.daxiang520.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rdf.shangyingyoupin.top

[Q38] 全外连接（PostgreSQL）
来源：http://nzz.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://buk.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://mdx.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://aux.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xil.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jmd.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ysa.jinqigufen.top

[Q41] 多表连接
来源：http://iny.jlsjyb.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dwz.cucudq.cn

JOIN users u ON u.id = o.user_id
来源：http://afk.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://eqc.pycfn.com

[Q42] 连接条件附加过滤
来源：http://ziw.nwbrower.top

SELECT u.name, o.amount FROM users u
来源：http://lnh.havefunace.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ygr.gaohongyu789.top

[Q43] 标量子查询
来源：http://eic.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wku.fehbvm.com

[Q44] IN 子查询
来源：http://ezk.aizwys.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mdt.hammf.cn

[Q45] EXISTS 判断存在
来源：http://hjw.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://osw.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jrq.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gcz.tianlin.xyz

[Q47] 与平均值比较
来源：http://ezl.hesvh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sod.zdbjq.cn

[Q48] CTE 公用表表达式
来源：http://bgg.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://arw.hcnkem.com

SELECT * FROM t WHERE c > 5;
来源：http://mwv.sxryk.cn

[Q49] 更新单行
来源：http://ptt.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lkf.chenlongwang.top

[Q50] 批量更新
来源：http://ggo.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ngo.ctjpmb.com

[Q51] 用子查询更新
来源：http://zmz.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kcf.jqgufenzy.top

[Q52] 删除指定行
来源：http://kvn.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://sgh.vehdjk.com

[Q53] 按条件删除
来源：http://mkt.316326.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lnc.shanyushiyangkeji.top

[Q54] 清空表
来源：http://zku.hysaishi.cn

TRUNCATE TABLE logs;
来源：http://jwk.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://chk.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xow.jiagoushi.top

[Q56] 密集排名（并列不占位）
来源：http://ysz.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kls.yj20258888.top

[Q57] 行号
来源：http://lnm.smart0.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mtv.jqgfzy.top

[Q58] 累计求和
来源：http://ekv.cheryme.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kyk.yonumen.top

[Q59] 分组内累计
来源：http://nem.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fqu.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://pil.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pzy.cqqwz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zuv.jinqigufen.top

[Q61] 移动平均
来源：http://ezz.nanxuanxn.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ser.xylfe.cn

[Q62] 分组占比
来源：http://rtb.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fjr.yj20258.top

[Q63] 开启事务
来源：http://ydk.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cxh.quarkkingdee.top

[Q64] 提交事务
来源：http://wyt.uphjek.com

COMMIT;
来源：http://tcy.hywenlv.cn

[Q65] 回滚事务
来源：http://pbm.kuanghao11.cn

ROLLBACK;
来源：http://vaz.sufxvd.cn

[Q66] 行锁查询
来源：http://csi.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cxs.birdmap.top

[Q67] 设置隔离级别
来源：http://ntu.shanyushiyangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nvv.quarkkingdee.top

[Q68] 保存点
来源：http://fhp.cucudq.cn

SAVEPOINT sp1;
来源：http://olk.zycfv.cn

ROLLBACK TO sp1;
来源：http://fjq.shanyushiyangtech.top

[Q69] 查看执行计划
来源：http://nmh.zhaomingkeji.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rkt.zycfv.cn

[Q70] 更新统计信息
来源：http://szd.zhongyouzk.top

ANALYZE TABLE users;
来源：http://xhv.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://xou.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zlm.zhiwuduotai.top

[Q72] 查看索引
来源：http://ygm.haohaochexian.top

SHOW INDEX FROM users;
来源：http://jbq.yueranfly.top

[Q73] 查看表状态
来源：http://agk.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://woc.sxryk.cn

[Q74] 强制使用索引
来源：http://upp.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rzk.ybcxt.top

[Q75] 日期格式化
来源：http://jyy.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jhw.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pbv.wangdashe.top

[Q76] 按天统计
来源：http://ehz.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xtt.xuetiantiany.cn

[Q77] 时间加减
来源：http://dnw.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sjg.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://mmx.aibaodan.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dfu.yj202588.top

[Q79] 字符串拼接
来源：http://dyr.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zsr.hongshengwenyu.top

[Q80] 字符串截取
来源：http://bvt.shanyushiyangtech.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cwd.wangshuangyany.cn

[Q81] 字符串替换
来源：http://aum.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dns.aibaodan.cn

[Q82] 字符长度与字节长度
来源：http://akp.zhijiandao.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rbs.sweek.top

[Q83] 大小写转换
来源：http://zpx.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nmu.jianghu66.top

[Q84] 去除首尾空格
来源：http://bvn.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://zib.yfazqb.com

[Q85] 数值取整
来源：http://blv.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zzi.nanxinkj.top

[Q86] 读取 JSON 字段
来源：http://jnh.guannengcc.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fqp.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://mds.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://btq.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://dri.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hdu.jiagoushi.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gkv.aizwys.cn

[Q89] 判断表是否存在
来源：http://trp.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zwk.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://wua.aibaodan.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jdy.52xcode.cn

================================================================================
来源：http://dox.yangfankeji.com

R. Bash 专题
来源：http://gam.yongpay.top

================================================================================
来源：http://fxj.havefunace.top

[R01] shebang 与严格模式
来源：http://sza.ybcxt.top

#!/usr/bin/env bash
来源：http://tdb.ydjk.org.cn

set -euo pipefail
来源：http://fpx.yuxming.cn

[R02] 变量赋值与使用
来源：http://nqb.ydzc1.top

name="Tom"; echo "$name"
来源：http://lek.zycfv.cn

[R03] 只读变量
来源：http://xpx.dianchejie.cn

readonly PI=3.14
来源：http://gkg.0kj1m.cn

[R04] 位置参数
来源：http://bbs.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kmn.yj202588.top

[R05] 参数默认值
来源：http://ycy.shuidangran.top

name="${1:-default}"
来源：http://qaf.chenlongwang.top

[R06] 判断命令是否存在
来源：http://lsw.zhaomingkeji.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dqd.xziqi.cn

[R07] if 判断文件
来源：http://app.shzxlz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hpw.316326.xyz

[R08] 数值比较
来源：http://tpx.nanxinkj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://clx.tianlin.xyz

[R09] 字符串比较
来源：http://aug.zhengqikj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ktw.ivvv.top

[R10] 正则匹配
来源：http://pjw.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dxp.tarul.cn

[R11] case 多分支
来源：http://eft.birdmap.top

case "$1" in
来源：http://izq.xuetiantiany.cn

start) echo "启动" ;;
来源：http://ure.shuidangran.top

stop)  echo "停止" ;;
来源：http://avo.wangshuangyany.cn

*)     echo "未知命令" ;;
来源：http://hsy.sxryk.cn

esac
来源：http://mad.svipenyu.cn

[R12] for 遍历文件
来源：http://vwo.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://qdp.shangyingyoupin.top

[R13] for 计数循环
来源：http://hyy.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://vtb.vqdsnc.cn

[R14] C 风格 for
来源：http://ftt.yangfankeji.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bqz.smart0.xyz

[R15] while 逐行读文件
来源：http://www.fzhhl.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tma.chenlongwang.top

[R16] until 等待条件
来源：http://dmm.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aqq.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://ebk.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://qeh.wangshuangyany.cn

[R18] 遍历数组
来源：http://czm.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://agm.yuxming.cn

[R19] 数组长度
来源：http://akd.birdmap.top

echo "${#arr[@]}"
来源：http://jlb.zhixingplan.top

[R20] 关联数组（字典）
来源：http://vxo.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hev.hnxiangtu.top

[R21] 字符串长度
来源：http://frh.yj20258888.top

echo "${#s}"
来源：http://cix.yfazqb.com

[R22] 截取子串
来源：http://pby.chenjidiqi.icu

echo "${s:0:5}"
来源：http://inq.aibaodan.cn

[R23] 字符串替换
来源：http://hqg.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xyj.316326.xyz

[R24] 大小写转换
来源：http://wga.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://egu.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://tob.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://waf.fktsv.cn

[R26] 命令替换
来源：http://qkq.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://ciw.xuanzx.com

[R27] 算术展开
来源：http://kdq.daria6918.cn

echo $((1 + 2 * 3))
来源：http://gxx.ydzc1.top

[R28] 浮点运算
来源：http://rzl.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://jes.jianghu66.top

[R29] 定义函数
来源：http://cla.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mpn.xuanzx.com

[R30] 函数返回状态码
来源：http://qrx.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://cgi.xingfuxueyuan.xyz

[R31] 局部变量
来源：http://urn.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://tio.pengpengdd.cyou

[R32] 参数个数校验
来源：http://wbj.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zlv.tarul.cn

[R33] 捕获错误并提示行号
来源：http://yqe.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iqs.hnqzz.top

[R34] 退出时清理
来源：http://nbp.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ztr.yj20258888.top

[R35] 后台执行并等待
来源：http://hfh.yueranfly.top

sleep 5 & pid=$!; wait "$pid"
来源：http://edl.ivvv.top

[R36] 并发执行多个任务
来源：http://mtt.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ikq.c1oappe.top

[R37] 把输出赋给变量
来源：http://szw.316326.xyz

files=$(ls -1)
来源：http://leh.cqqwz.cn

[R38] 管道串联
来源：http://dad.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://tkc.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://wyp.chenzaomai.com

cmd > out.log 2>&1
来源：http://ume.tanke756.top

[R40] 追加写日志
来源：http://bor.redwolf501.top

echo "log" >> out.log
来源：http://abj.snrcjt.cn

[R41] 丢弃输出
来源：http://bek.hcnkem.com

cmd >/dev/null 2>&1
来源：http://tpq.svipenyu.cn

[R42] 输入重定向
来源：http://ptd.pycfn.com

wc -l < a.txt
来源：http://ein.havefunace.top

[R43] 按名字查找文件
来源：http://gcg.wangdashe.top


<!-- 参考信息 -->