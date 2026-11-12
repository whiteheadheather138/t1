代发 wailian999

================================================================================
来源：http://nub.jinqigufen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wpr.gogol.net.cn

================================================================================
来源：http://cdl.ybcxt.top

[Q01] 创建表
来源：http://lqa.birdmap.top

CREATE TABLE users (
来源：http://opl.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uem.yuanzhike.top

name VARCHAR(50) NOT NULL,
来源：http://kdb.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://ifu.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uav.jinqigufen.top

);
来源：http://auw.hcnkem.com

[Q02] 创建带外键的表
来源：http://qag.guannengcc.top

CREATE TABLE orders (
来源：http://aaa.meibo888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eqv.zhiwuduotai.top

user_id INT NOT NULL,
来源：http://itd.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://bxw.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ynn.ivvv.top

);
来源：http://nru.haohaochexian.top

[Q03] 增加列
来源：http://nhn.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fvk.redwolf501.top

[Q04] 修改列类型
来源：http://oyr.feifeiyinyue.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wax.epnwcf.com

[Q05] 重命名列
来源：http://rdz.guowangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mpa.jinyuanbaomall.cn

[Q06] 删除列
来源：http://qdx.sufxvd.cn

ALTER TABLE users DROP COLUMN age;
来源：http://unw.xinyue.icu

[Q07] 删除表
来源：http://jie.xylfe.cn

DROP TABLE IF EXISTS orders;
来源：http://uyh.hammf.cn

[Q08] 创建普通索引
来源：http://owy.xuanzx.com

CREATE INDEX idx_users_email ON users(email);
来源：http://qdx.yuanzhike.top

[Q09] 创建唯一索引
来源：http://xjk.jqgufenzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ysk.daria6918.cn

[Q10] 插入单行
来源：http://kur.shuidangran.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tjw.gotoacloud.top

[Q11] 一次插入多行
来源：http://krq.haohaochexian.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vsm.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://jvt.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gbm.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ggb.zhiwuduotai.top

[Q13] 忽略重复插入
来源：http://gmz.nanxuanxn.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oly.sweek.top

[Q14] 存在则更新（upsert）
来源：http://xev.0kj1m.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ufm.zhiwuduotai.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fzl.ydjk.org.cn

[Q15] 查询全部
来源：http://dtn.yuanzhike.top

SELECT * FROM users;
来源：http://nse.xinyue.icu

[Q16] 查询指定列
来源：http://xnk.nanxuanxn.top

SELECT id, name FROM users;
来源：http://pgo.ehwqpu.com

[Q17] 条件查询
来源：http://pxp.jqgfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://syg.wangshuangyany.cn

[Q18] 模糊匹配
来源：http://fef.redwolf501.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uvh.gaohongyu789.top

[Q19] 范围查询
来源：http://lnp.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kwx.fktsv.cn

[Q20] IN 列表
来源：http://eif.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://glt.zdqjudy.top

[Q21] 空值判断
来源：http://eci.xinyue.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://zml.hywenlv.cn

[Q22] 排序
来源：http://xav.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ned.tanke756.top

[Q23] 分页
来源：http://xve.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jar.bbcook.cn

[Q24] 去重
来源：http://bua.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://ktf.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://mua.jinghuilouyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yjg.xinyue.icu

[Q26] 计数
来源：http://ynx.yuxming.cn

SELECT COUNT(*) FROM users;
来源：http://siw.hysaishi.cn

[Q27] 条件计数
来源：http://omm.yanxiufei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vhd.shangyingyoupin.top

[Q28] 求和与平均
来源：http://hou.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mgx.jqgufenzy.top

[Q29] 最大最小值
来源：http://hzx.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://hat.hfpthk.cn

[Q30] 分组统计
来源：http://xmf.yj20258888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yur.chenzaomai.com

[Q31] 分组后过滤
来源：http://emf.svipenyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zul.yonumen.top

[Q32] 分组拼接字符串
来源：http://dup.yonumen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fmk.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vhu.jqgufenzy.top

[Q33] 多列分组
来源：http://qge.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vsq.jinqigufen.top

[Q34] 每组取第一条
来源：http://uls.dashuyun.cn

SELECT * FROM (
来源：http://pfo.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fzd.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://hiv.ydjk.org.cn

[Q35] 内连接
来源：http://gvt.jianghu66.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://emy.zycfv.cn

[Q36] 左连接
来源：http://tgq.zhijiandao.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wpp.wangdashe.top

[Q37] 右连接
来源：http://gce.ctjpmb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wkr.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://rlq.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://enp.hammf.cn

[Q39] 自连接（查上下级）
来源：http://xah.mhx1999.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xro.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iod.feifeiyinyue.top

[Q40] 交叉连接（笛卡尔积）
来源：http://guc.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ged.shanyushiyangtech.top

[Q41] 多表连接
来源：http://olm.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qef.yuanzhike.top

JOIN users u ON u.id = o.user_id
来源：http://rkd.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://jlo.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://apk.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://ioc.sysykeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nrj.9152youxi.cn

[Q43] 标量子查询
来源：http://sdr.hywenlv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vku.jinqigufen.top

[Q44] IN 子查询
来源：http://mvj.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xhi.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://yhy.ppjwa.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mrp.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gai.ydjk.org.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hvc.mhx1999.top

[Q47] 与平均值比较
来源：http://saf.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hci.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://qmx.ivvv.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zqz.nwbrower.top

SELECT * FROM t WHERE c > 5;
来源：http://gsg.shuidangran.top

[Q49] 更新单行
来源：http://hoe.quarkkingdee.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aks.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://wsz.zdqjudy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fkm.yueranfly.top

[Q51] 用子查询更新
来源：http://crh.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vsw.tanke756.top

[Q52] 删除指定行
来源：http://gcw.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://gtk.nanxuanxn.top

[Q53] 按条件删除
来源：http://ady.xuanzx.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://csm.tanke756.top

[Q54] 清空表
来源：http://daw.bjfxy.top

TRUNCATE TABLE logs;
来源：http://yow.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://upz.yj20258.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dxp.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://giz.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tjf.vqdsnc.cn

[Q57] 行号
来源：http://mem.guannengcc.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qlc.hywenlv.cn

[Q58] 累计求和
来源：http://sfe.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zsw.xuanzx.com

[Q59] 分组内累计
来源：http://kuc.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kzq.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://xlu.hfpthk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iht.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rrj.zhixingplan.top

[Q61] 移动平均
来源：http://kzb.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xqo.yuanzhike.top

[Q62] 分组占比
来源：http://elw.daxiang520.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sih.ywan-chungtsiang.top

[Q63] 开启事务
来源：http://pbe.vqdsnc.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://num.ydzc1.top

[Q64] 提交事务
来源：http://ifw.ydzc1.top

COMMIT;
来源：http://znl.wangdashe.top

[Q65] 回滚事务
来源：http://gdz.kuanghao11.cn

ROLLBACK;
来源：http://brx.yangfankeji.com

[Q66] 行锁查询
来源：http://wwg.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fjz.gogol.net.cn

[Q67] 设置隔离级别
来源：http://vcs.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://geb.jiagoushi.top

[Q68] 保存点
来源：http://bbg.aizwys.cn

SAVEPOINT sp1;
来源：http://tdw.shanyushiyangtech.top

ROLLBACK TO sp1;
来源：http://hsz.vehdjk.com

[Q69] 查看执行计划
来源：http://pbt.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nec.pengpengdd.cyou

[Q70] 更新统计信息
来源：http://vvm.guowangkeji.top

ANALYZE TABLE users;
来源：http://chk.bbcook.cn

[Q71] 查看建表语句
来源：http://qoe.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tvs.dianchejie.cn

[Q72] 查看索引
来源：http://eft.hnxiangtu.top

SHOW INDEX FROM users;
来源：http://rnc.tian-w.cn

[Q73] 查看表状态
来源：http://qne.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://iho.0kj1m.cn

[Q74] 强制使用索引
来源：http://ihr.tanke756.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ycr.zhijiandao.cn

[Q75] 日期格式化
来源：http://uqf.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dzs.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pux.sysykeji.top

[Q76] 按天统计
来源：http://cpo.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://faj.jianghu66.top

[Q77] 时间加减
来源：http://oyk.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bzv.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://qej.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zwc.gotoacloud.top

[Q79] 字符串拼接
来源：http://xza.zdbjq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lox.jlsjyb.cn

[Q80] 字符串截取
来源：http://cpy.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mst.chenzaomai.com

[Q81] 字符串替换
来源：http://tpc.zdqjudy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nfs.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://cte.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ise.zhongyouzk.top

[Q83] 大小写转换
来源：http://gfq.sufxvd.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zxb.iojbl.cn

[Q84] 去除首尾空格
来源：http://mla.guowangkeji.top

SELECT TRIM(name) FROM users;
来源：http://tlp.snrcjt.cn

[Q85] 数值取整
来源：http://xlz.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fcm.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://hdt.sweek.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bqz.gzhubu.top

[Q87] JSON 字段做条件
来源：http://drp.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://reo.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://awb.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pvr.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kqj.jinyuanbaomall.cn

[Q89] 判断表是否存在
来源：http://iay.zdqjudy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vlq.mhx1999.top

[Q90] 生成序号列
来源：http://lue.hammf.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cah.shanyushiyangkeji.top

================================================================================
来源：http://eod.mhx1999.top

R. Bash 专题
来源：http://uli.shanyushiyangkeji.top

================================================================================
来源：http://jey.tian-w.cn

[R01] shebang 与严格模式
来源：http://fnx.xinyue.icu

#!/usr/bin/env bash
来源：http://iwx.hongshengwenyu.top

set -euo pipefail
来源：http://zvn.9152youxi.cn

[R02] 变量赋值与使用
来源：http://glk.aibaodan.cn

name="Tom"; echo "$name"
来源：http://vry.pycfn.com

[R03] 只读变量
来源：http://zzk.yuxming.cn

readonly PI=3.14
来源：http://jqh.yj202588.top

[R04] 位置参数
来源：http://bbc.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hjx.sysykeji.top

[R05] 参数默认值
来源：http://aoa.epnwcf.com

name="${1:-default}"
来源：http://jbt.meibo888.top

[R06] 判断命令是否存在
来源：http://qtp.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qwd.tianlin.xyz

[R07] if 判断文件
来源：http://bup.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aqw.xylfe.cn

[R08] 数值比较
来源：http://hhw.zhengqikj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lhr.shangyingyoupin.top

[R09] 字符串比较
来源：http://asw.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ldv.tarul.cn

[R10] 正则匹配
来源：http://dew.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tiy.xuanzx.com

[R11] case 多分支
来源：http://ugt.pycfn.com

case "$1" in
来源：http://bgu.fengsongda.top

start) echo "启动" ;;
来源：http://nms.vqdsnc.cn

stop)  echo "停止" ;;
来源：http://ijy.ydjk.org.cn

*)     echo "未知命令" ;;
来源：http://yvx.bbcook.cn

esac
来源：http://njg.aizwys.cn

[R12] for 遍历文件
来源：http://tyj.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://foe.jinqigufen.top

[R13] for 计数循环
来源：http://vht.zhijiandao.cn

for i in {1..10}; do echo "$i"; done
来源：http://mdt.dashuyun.cn

[R14] C 风格 for
来源：http://jru.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dao.zdbjq.cn

[R15] while 逐行读文件
来源：http://jyf.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zec.meibo888.top

[R16] until 等待条件
来源：http://guq.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bmu.sweek.top

[R17] 数组定义与取值
来源：http://aqj.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://pit.jinghuilouyu.cn

[R18] 遍历数组
来源：http://xck.ydzc1.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fyd.cqqwz.cn

[R19] 数组长度
来源：http://jmt.nanxinkj.top

echo "${#arr[@]}"
来源：http://zqr.hnxiangtu.top

[R20] 关联数组（字典）
来源：http://byq.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rbi.fanxiaobao.xyz

[R21] 字符串长度
来源：http://mbo.kuanghao11.cn

echo "${#s}"
来源：http://ikq.hnqzz.top

[R22] 截取子串
来源：http://hec.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://xie.cqqwz.cn

[R23] 字符串替换
来源：http://ige.yj202588.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://our.zhengqikj.top

[R24] 大小写转换
来源：http://nvu.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://oze.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://eyj.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://snk.guannengcc.top

[R26] 命令替换
来源：http://pnh.hcnkem.com

now=$(date +%F); echo "$now"
来源：http://tog.ywan-chungtsiang.top

[R27] 算术展开
来源：http://pfj.epnwcf.com

echo $((1 + 2 * 3))
来源：http://nru.c1oappe.top

[R28] 浮点运算
来源：http://wvx.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://ojw.pycfn.com

[R29] 定义函数
来源：http://crs.nanxinkj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://exq.52xcode.cn

[R30] 函数返回状态码
来源：http://tfq.hcnkem.com

f() { return 0; }; f || echo "失败了"
来源：http://viq.sxryk.cn

[R31] 局部变量
来源：http://cqf.jinyuanbaomall.cn

f() { local x=1; echo "$x"; }
来源：http://fcp.xinyue.icu

[R32] 参数个数校验
来源：http://tmo.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://goz.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://dsp.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rnu.jqgfzy.top

[R34] 退出时清理
来源：http://rnk.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://uvs.dashuyun.cn

[R35] 后台执行并等待
来源：http://axo.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://vfe.cashguo.top

[R36] 并发执行多个任务
来源：http://nwg.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://huy.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://kdt.shangyingyoupin.top

files=$(ls -1)
来源：http://jkz.hysaishi.cn

[R38] 管道串联
来源：http://szk.bjfxy.top

cat a.txt | grep -i error | wc -l
来源：http://beg.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://kda.yanxiufei.cn

cmd > out.log 2>&1
来源：http://mwi.cheryme.top

[R40] 追加写日志
来源：http://emw.fengsongda.top

echo "log" >> out.log
来源：http://htz.jinqigfzy.top

[R41] 丢弃输出
来源：http://zjl.jinghuilouyu.cn

cmd >/dev/null 2>&1
来源：http://dpw.aizwys.cn

[R42] 输入重定向
来源：http://nsv.jqgfzy.top

wc -l < a.txt
来源：http://jlg.tarul.cn

[R43] 按名字查找文件
来源：http://yrj.fanxiaobao.xyz


<!-- 参考信息 -->