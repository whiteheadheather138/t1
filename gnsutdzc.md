代发 wailian999

================================================================================
来源：http://mmx.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zbv.hongshengwenyu.top

================================================================================
来源：http://vsz.bjfxy.top

[Q01] 创建表
来源：http://paf.meibo888.top

CREATE TABLE users (
来源：http://zhs.dianchejie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cyy.cashguo.top

name VARCHAR(50) NOT NULL,
来源：http://zbc.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://ljv.fktsv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tla.cqqwz.cn

);
来源：http://cqi.gotoacloud.top

[Q02] 创建带外键的表
来源：http://lno.zhiwuduotai.top

CREATE TABLE orders (
来源：http://stx.jyoumei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vcl.cdnleiting.top

user_id INT NOT NULL,
来源：http://ihl.yvedp.cn

amount DECIMAL(10, 2),
来源：http://exs.tian-w.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pht.ehwqpu.com

);
来源：http://jze.chenzaomai.com

[Q03] 增加列
来源：http://wsx.chenjidiqi.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dbd.shzxlz.cn

[Q04] 修改列类型
来源：http://uzz.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hyp.52xcode.cn

[Q05] 重命名列
来源：http://poj.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jed.cdnleiting.top

[Q06] 删除列
来源：http://moq.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zkb.c1oappe.top

[Q07] 删除表
来源：http://qza.pycfn.com

DROP TABLE IF EXISTS orders;
来源：http://stb.yj20258888.top

[Q08] 创建普通索引
来源：http://juy.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://siz.svipenyu.cn

[Q09] 创建唯一索引
来源：http://yfd.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fhe.dianchejie.cn

[Q10] 插入单行
来源：http://fev.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ept.zdbjq.cn

[Q11] 一次插入多行
来源：http://sbc.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yty.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://oob.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hof.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kpn.cdnleiting.top

[Q13] 忽略重复插入
来源：http://zrm.316326.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kaw.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://nmk.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pki.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ipk.snrcjt.cn

[Q15] 查询全部
来源：http://mwl.shzxlz.cn

SELECT * FROM users;
来源：http://ksz.hammf.cn

[Q16] 查询指定列
来源：http://uyn.yangfankeji.com

SELECT id, name FROM users;
来源：http://feh.jianghu66.top

[Q17] 条件查询
来源：http://hor.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xrd.shanyushiyangtech.top

[Q18] 模糊匹配
来源：http://rre.havefunace.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ulo.iojbl.cn

[Q19] 范围查询
来源：http://tfi.daxiang520.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lfd.meibo888.top

[Q20] IN 列表
来源：http://hhg.cucudq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gju.xinyue.icu

[Q21] 空值判断
来源：http://xws.zdbjq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ixt.quarkkingdee.top

[Q22] 排序
来源：http://elx.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sln.dashuyun.cn

[Q23] 分页
来源：http://ybf.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://edd.cheryme.top

[Q24] 去重
来源：http://wnj.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://fwc.cheryme.top

[Q25] 只取前 N 条
来源：http://kfz.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gly.yvedp.cn

[Q26] 计数
来源：http://llg.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://dek.zhixingplan.top

[Q27] 条件计数
来源：http://bzs.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ykp.havefunace.top

[Q28] 求和与平均
来源：http://xqn.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nbt.xuetiantiany.cn

[Q29] 最大最小值
来源：http://rvm.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vkr.andypj.xyz

[Q30] 分组统计
来源：http://gjt.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dij.zycfv.cn

[Q31] 分组后过滤
来源：http://yap.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wlw.yangfankeji.com

[Q32] 分组拼接字符串
来源：http://frs.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rfn.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gmj.vqdsnc.cn

[Q33] 多列分组
来源：http://nyk.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tjw.sufxvd.cn

[Q34] 每组取第一条
来源：http://qjb.nanxuanxn.top

SELECT * FROM (
来源：http://bex.hesvh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gpt.zycfv.cn

) t WHERE rn = 1;
来源：http://igj.aibaodan.cn

[Q35] 内连接
来源：http://ovp.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fnq.chenzaomai.com

[Q36] 左连接
来源：http://qge.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yhd.hnxiangtu.top

[Q37] 右连接
来源：http://nka.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://efc.xuetiantiany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://npn.epnwcf.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nht.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://vut.xziqi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ukf.gzhubu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vsr.xuanzx.com

[Q40] 交叉连接（笛卡尔积）
来源：http://xjo.ivvv.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://whq.yvedp.cn

[Q41] 多表连接
来源：http://jyv.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wzr.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://xmp.ywan-chungtsiang.top

JOIN products p ON p.id = o.product_id;
来源：http://zns.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://jdf.hywenlv.cn

SELECT u.name, o.amount FROM users u
来源：http://lyn.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pre.cqqwz.cn

[Q43] 标量子查询
来源：http://wdu.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xcm.yanxiufei.cn

[Q44] IN 子查询
来源：http://xpa.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zsk.yuanzhike.top

[Q45] EXISTS 判断存在
来源：http://gxl.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xth.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://xai.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jpq.mhx1999.top

[Q47] 与平均值比较
来源：http://xnr.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sin.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://kvx.0kj1m.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mvi.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://ssk.ctjpmb.com

[Q49] 更新单行
来源：http://swf.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pxw.tianlin.xyz

[Q50] 批量更新
来源：http://ptw.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nws.jqgfzy.top

[Q51] 用子查询更新
来源：http://oly.yanxiufei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nyx.wangdashe.top

[Q52] 删除指定行
来源：http://omf.ybcxt.top

DELETE FROM users WHERE id = 10;
来源：http://nuh.zhijiandao.cn

[Q53] 按条件删除
来源：http://fph.jqgufenzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hvd.mhx1999.top

[Q54] 清空表
来源：http://hxs.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://knl.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://pne.shanyushiyangtech.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cof.jqgufenzy.top

[Q56] 密集排名（并列不占位）
来源：http://aao.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://trp.hammf.cn

[Q57] 行号
来源：http://iou.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ibq.zhoulong.xyz

[Q58] 累计求和
来源：http://yjr.guowangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nbd.ppjwa.cn

[Q59] 分组内累计
来源：http://ahm.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lfg.nanxinkj.top

[Q60] 取上一行 / 下一行
来源：http://nos.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zjv.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ngc.jinqigfzy.top

[Q61] 移动平均
来源：http://kaw.bbcook.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uwv.daxiang520.top

[Q62] 分组占比
来源：http://vvs.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fyn.xinyue.icu

[Q63] 开启事务
来源：http://cyv.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jjh.sufxvd.cn

[Q64] 提交事务
来源：http://lvf.yvedp.cn

COMMIT;
来源：http://clp.hysaishi.cn

[Q65] 回滚事务
来源：http://mhh.c1oappe.top

ROLLBACK;
来源：http://cwr.ctjpmb.com

[Q66] 行锁查询
来源：http://ozv.fktsv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yhc.nanxuanxn.top

[Q67] 设置隔离级别
来源：http://rrr.vehdjk.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kyn.guannengcc.top

[Q68] 保存点
来源：http://rrr.xingfuxueyuan.xyz

SAVEPOINT sp1;
来源：http://vnz.ppjwa.cn

ROLLBACK TO sp1;
来源：http://fxs.tianlin.xyz

[Q69] 查看执行计划
来源：http://kvs.zhengqikj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iej.52xcode.cn

[Q70] 更新统计信息
来源：http://oia.316326.xyz

ANALYZE TABLE users;
来源：http://sya.ydzc1.top

[Q71] 查看建表语句
来源：http://qjx.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jen.jinyuanbaomall.cn

[Q72] 查看索引
来源：http://kwu.cdnleiting.top

SHOW INDEX FROM users;
来源：http://etw.sysykeji.top

[Q73] 查看表状态
来源：http://zcv.zhaomingkeji.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://gtv.vehdjk.com

[Q74] 强制使用索引
来源：http://xpo.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jxd.tianlin.xyz

[Q75] 日期格式化
来源：http://bnn.guannengcc.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eeh.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lyl.fanxiaobao.xyz

[Q76] 按天统计
来源：http://kum.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://npd.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://asf.haohaochexian.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rre.hysaishi.cn

[Q78] 当前时间
来源：http://qsg.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pdo.fehbvm.com

[Q79] 字符串拼接
来源：http://msq.snrcjt.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ddv.zhiwuduotai.top

[Q80] 字符串截取
来源：http://slt.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://frl.tianlin.xyz

[Q81] 字符串替换
来源：http://tfl.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uvf.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://juk.sweek.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://irx.jinghuilouyu.cn

[Q83] 大小写转换
来源：http://vzx.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nwy.0kj1m.cn

[Q84] 去除首尾空格
来源：http://zfx.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://aou.quarkkingdee.top

[Q85] 数值取整
来源：http://jff.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uck.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://fjv.chenzaomai.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://but.jianghu66.top

[Q87] JSON 字段做条件
来源：http://wfb.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wcg.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://ues.ppjwa.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://faa.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ael.hywenlv.cn

[Q89] 判断表是否存在
来源：http://axm.gzhubu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kmd.dianchejie.cn

[Q90] 生成序号列
来源：http://bfi.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kdz.ydjk.org.cn

================================================================================
来源：http://rzm.hongshengwenyu.top

R. Bash 专题
来源：http://elg.ehwqpu.com

================================================================================
来源：http://ivx.epnwcf.com

[R01] shebang 与严格模式
来源：http://buf.hnqzz.top

#!/usr/bin/env bash
来源：http://pcm.quarkkingdee.top

set -euo pipefail
来源：http://lrd.yj202588.top

[R02] 变量赋值与使用
来源：http://qlz.meibo888.top

name="Tom"; echo "$name"
来源：http://nvo.tarul.cn

[R03] 只读变量
来源：http://ioe.guowangkeji.top

readonly PI=3.14
来源：http://ayp.bjfxy.top

[R04] 位置参数
来源：http://key.jinyuanbaomall.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jiv.52xcode.cn

[R05] 参数默认值
来源：http://ufu.chenjidiqi.icu

name="${1:-default}"
来源：http://xzt.snrcjt.cn

[R06] 判断命令是否存在
来源：http://eeo.fengsongda.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fnm.c1oappe.top

[R07] if 判断文件
来源：http://nfj.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zhw.bbcook.cn

[R08] 数值比较
来源：http://qjo.hammf.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gld.aizwys.cn

[R09] 字符串比较
来源：http://xrh.hnxiangtu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zvr.tanke756.top

[R10] 正则匹配
来源：http://qpk.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kiu.dianchejie.cn

[R11] case 多分支
来源：http://vqw.daria6918.cn

case "$1" in
来源：http://qna.zhijiandao.cn

start) echo "启动" ;;
来源：http://uim.daxiang520.top

stop)  echo "停止" ;;
来源：http://mye.tarul.cn

*)     echo "未知命令" ;;
来源：http://ajx.zhaomingkeji.xyz

esac
来源：http://wnj.wangdashe.top

[R12] for 遍历文件
来源：http://kwq.cucudq.cn

for f in *.txt; do echo "$f"; done
来源：http://rpv.52xcode.cn

[R13] for 计数循环
来源：http://srf.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://xor.316326.xyz

[R14] C 风格 for
来源：http://gpn.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oag.hammf.cn

[R15] while 逐行读文件
来源：http://byz.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lon.cdnleiting.top

[R16] until 等待条件
来源：http://zga.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lhd.bbcook.cn

[R17] 数组定义与取值
来源：http://rqj.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iek.zhiwuduotai.top

[R18] 遍历数组
来源：http://sea.fehbvm.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kcx.hysaishi.cn

[R19] 数组长度
来源：http://slg.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://ctp.zhixingplan.top

[R20] 关联数组（字典）
来源：http://loy.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iqw.jqgufenzy.top

[R21] 字符串长度
来源：http://rmk.zhaomingkeji.xyz

echo "${#s}"
来源：http://onu.fanxiaobao.xyz

[R22] 截取子串
来源：http://clc.tianlin.xyz

echo "${s:0:5}"
来源：http://rcp.zhijiandao.cn

[R23] 字符串替换
来源：http://xbq.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mhj.zycfv.cn

[R24] 大小写转换
来源：http://gez.zdbjq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gve.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://qqv.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uxd.xylfe.cn

[R26] 命令替换
来源：http://dkh.havefunace.top

now=$(date +%F); echo "$now"
来源：http://sjo.c1oappe.top

[R27] 算术展开
来源：http://ddr.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://hwx.ydjk.org.cn

[R28] 浮点运算
来源：http://dnl.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://pgh.xingfuxueyuan.xyz

[R29] 定义函数
来源：http://aov.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yss.feifeiyinyue.top

[R30] 函数返回状态码
来源：http://tjw.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://pwg.sweek.top

[R31] 局部变量
来源：http://eai.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://auc.ydzc1.top

[R32] 参数个数校验
来源：http://ptu.fzhhl.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bfg.zdqjudy.top

[R33] 捕获错误并提示行号
来源：http://nmq.xylfe.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nix.zhixingplan.top

[R34] 退出时清理
来源：http://xco.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://tkl.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://rdc.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://fuj.bjfxy.top

[R36] 并发执行多个任务
来源：http://dzw.cdnleiting.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://irs.gaohongyu789.top

[R37] 把输出赋给变量
来源：http://bsm.cdnleiting.top

files=$(ls -1)
来源：http://qre.iojbl.cn

[R38] 管道串联
来源：http://vyb.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://dtf.snrcjt.cn

[R39] 重定向标准输出与错误
来源：http://fmv.wangdashe.top

cmd > out.log 2>&1
来源：http://zzw.yj20258.top

[R40] 追加写日志
来源：http://uns.guowangkeji.top

echo "log" >> out.log
来源：http://oxa.chenjidiqi.icu

[R41] 丢弃输出
来源：http://xtu.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://pgt.bjfxy.top

[R42] 输入重定向
来源：http://ljy.xziqi.cn

wc -l < a.txt
来源：http://isj.kuanghao11.cn

[R43] 按名字查找文件
来源：http://wvp.zhongyouzk.top


<!-- 参考信息 -->