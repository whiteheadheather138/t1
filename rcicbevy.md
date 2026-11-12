代发 wailian999

CREATE TABLE users (
来源：http://nyk.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vlf.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://xfz.meibo888.top

email VARCHAR(100) UNIQUE,
来源：http://cqm.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dnk.gogol.net.cn

);
来源：http://diy.hammf.cn

[Q02] 创建带外键的表
来源：http://kuc.zhijiandao.cn

CREATE TABLE orders (
来源：http://mro.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://chz.meibo888.top

user_id INT NOT NULL,
来源：http://edx.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://hoh.sysykeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gen.ppjwa.cn

);
来源：http://kqb.jqgfzy.top

[Q03] 增加列
来源：http://tfe.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ptq.yj20258.top

[Q04] 修改列类型
来源：http://zme.chenlongwang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mtl.mhx1999.top

[Q05] 重命名列
来源：http://bao.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nlj.birdmap.top

[Q06] 删除列
来源：http://zaa.yj202588.top

ALTER TABLE users DROP COLUMN age;
来源：http://jbi.wangdashe.top

[Q07] 删除表
来源：http://zwl.uphjek.com

DROP TABLE IF EXISTS orders;
来源：http://tph.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://uim.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://lro.wangdashe.top

[Q09] 创建唯一索引
来源：http://lzq.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fik.zhoulong.xyz

[Q10] 插入单行
来源：http://iqn.sysykeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://grn.xziqi.cn

[Q11] 一次插入多行
来源：http://vsz.yj20258.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://syp.epnwcf.com

[Q12] 插入后取自增 ID
来源：http://shk.xuanzx.com

INSERT INTO users (name) VALUES ('C');
来源：http://wyl.zdbjq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qga.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://flf.smart0.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pwt.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://wra.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ogy.yuanzhike.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vzn.tian-w.cn

[Q15] 查询全部
来源：http://pju.birdmap.top

SELECT * FROM users;
来源：http://usr.shangyingyoupin.top

[Q16] 查询指定列
来源：http://wvm.cucudq.cn

SELECT id, name FROM users;
来源：http://psy.ivvv.top

[Q17] 条件查询
来源：http://xph.jqgfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jlg.zhengqikj.top

[Q18] 模糊匹配
来源：http://uki.guannengcc.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qyc.ppjwa.cn

[Q19] 范围查询
来源：http://vwh.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://grm.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://maj.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kzz.feifeiyinyue.top

[Q21] 空值判断
来源：http://avh.zdbjq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ebm.fktsv.cn

[Q22] 排序
来源：http://vqs.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jov.ivvv.top

[Q23] 分页
来源：http://owj.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pkt.ppjwa.cn

[Q24] 去重
来源：http://vfn.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://tov.daria6918.cn

[Q25] 只取前 N 条
来源：http://uhc.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zbk.chenzaomai.com

[Q26] 计数
来源：http://ehs.epnwcf.com

SELECT COUNT(*) FROM users;
来源：http://fwt.sjlbkw.cn

[Q27] 条件计数
来源：http://lbp.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zjh.tanke756.top

[Q28] 求和与平均
来源：http://jxm.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xfi.jqgfzy.top

[Q29] 最大最小值
来源：http://kue.zycfv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qon.chenzaomai.com

[Q30] 分组统计
来源：http://jjr.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hsi.tian-w.cn

[Q31] 分组后过滤
来源：http://rwf.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vil.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://dmh.hesvh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qvi.feifeiyinyue.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gwh.fengsongda.top

[Q33] 多列分组
来源：http://njy.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lus.hammf.cn

[Q34] 每组取第一条
来源：http://cew.cdnleiting.top

SELECT * FROM (
来源：http://bcq.ybcxt.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mok.sufxvd.cn

) t WHERE rn = 1;
来源：http://nml.aibaodan.cn

[Q35] 内连接
来源：http://jfi.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mto.ydzc1.top

[Q36] 左连接
来源：http://ldb.nanxinkj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tzw.yj20258888.top

[Q37] 右连接
来源：http://goe.sysykeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ewc.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://dbr.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vaf.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://kpj.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dsd.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jzy.ydjk.org.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://urc.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fkt.vehdjk.com

[Q41] 多表连接
来源：http://cjp.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://uav.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://wop.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://vgt.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://nrl.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://bhi.meibo888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://agq.daria6918.cn

[Q43] 标量子查询
来源：http://uxt.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vob.fktsv.cn

[Q44] IN 子查询
来源：http://heu.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eiz.birdmap.top

[Q45] EXISTS 判断存在
来源：http://qjx.pycfn.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tyw.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://jnx.bbcook.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yee.tarul.cn

[Q47] 与平均值比较
来源：http://gcz.nwbrower.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fto.yfazqb.com

[Q48] CTE 公用表表达式
来源：http://biy.svipenyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mzy.ydjk.org.cn

SELECT * FROM t WHERE c > 5;
来源：http://rfd.yangfankeji.com

[Q49] 更新单行
来源：http://pmz.xingfuxueyuan.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hxh.jinghuilouyu.cn

[Q50] 批量更新
来源：http://tjh.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bkj.quarkkingdee.top

[Q51] 用子查询更新
来源：http://zwx.xinyue.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rie.birdmap.top

[Q52] 删除指定行
来源：http://hso.yuxming.cn

DELETE FROM users WHERE id = 10;
来源：http://xsj.yj20258.top

[Q53] 按条件删除
来源：http://wdm.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xmg.sxryk.cn

[Q54] 清空表
来源：http://krl.sysykeji.top

TRUNCATE TABLE logs;
来源：http://dbn.yvedp.cn

[Q55] 排名（并列占位）
来源：http://lhh.iojbl.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eiz.chenjidiqi.icu

[Q56] 密集排名（并列不占位）
来源：http://ctg.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uuy.shanyushiyangkeji.top

[Q57] 行号
来源：http://rwp.guannengcc.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vjq.sysykeji.top

[Q58] 累计求和
来源：http://nbj.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dmr.sweek.top

[Q59] 分组内累计
来源：http://bvv.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bma.shangyingyoupin.top

[Q60] 取上一行 / 下一行
来源：http://hzi.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gtg.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ghj.uphjek.com

[Q61] 移动平均
来源：http://trj.jinqigufen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ovb.cheryme.top

[Q62] 分组占比
来源：http://cgx.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://trv.cucudq.cn

[Q63] 开启事务
来源：http://jee.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gjh.xziqi.cn

[Q64] 提交事务
来源：http://rgb.sysykeji.top

COMMIT;
来源：http://tpf.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://bpz.xziqi.cn

ROLLBACK;
来源：http://ffk.epnwcf.com

[Q66] 行锁查询
来源：http://mod.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://azz.0kj1m.cn

[Q67] 设置隔离级别
来源：http://klt.jinyuanbaomall.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hxt.cucudq.cn

[Q68] 保存点
来源：http://unp.sufxvd.cn

SAVEPOINT sp1;
来源：http://jgy.hesvh.cn

ROLLBACK TO sp1;
来源：http://ltn.yuxming.cn

[Q69] 查看执行计划
来源：http://qvz.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ybk.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://kov.mhx1999.top

ANALYZE TABLE users;
来源：http://xkx.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://uun.zycfv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tid.mhx1999.top

[Q72] 查看索引
来源：http://uej.yuxming.cn

SHOW INDEX FROM users;
来源：http://hyt.aibaodan.cn

[Q73] 查看表状态
来源：http://bzv.epnwcf.com

SHOW TABLE STATUS LIKE 'users';
来源：http://xfu.c1oappe.top

[Q74] 强制使用索引
来源：http://akj.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hpr.hfpthk.cn

[Q75] 日期格式化
来源：http://mfv.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gzp.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://izr.sysykeji.top

[Q76] 按天统计
来源：http://tsq.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vyi.cdnleiting.top

[Q77] 时间加减
来源：http://wdr.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yvn.52xcode.cn

[Q78] 当前时间
来源：http://zqw.birdmap.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nxd.smart0.xyz

[Q79] 字符串拼接
来源：http://spy.guannengcc.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rud.haohaochexian.top

[Q80] 字符串截取
来源：http://hvq.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://szj.mhx1999.top

[Q81] 字符串替换
来源：http://dnr.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qzj.redwolf501.top

[Q82] 字符长度与字节长度
来源：http://twl.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://irl.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://cnz.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://okr.daxiang520.top

[Q84] 去除首尾空格
来源：http://bqq.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://fwi.haohaochexian.top

[Q85] 数值取整
来源：http://onz.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://suv.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://ptv.iojbl.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bdh.yuxming.cn

[Q87] JSON 字段做条件
来源：http://vkt.yj20258.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xxw.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://vvk.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xgj.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tnf.dashuyun.cn

[Q89] 判断表是否存在
来源：http://opw.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jnr.zhengqikj.top

[Q90] 生成序号列
来源：http://jde.aibaodan.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dzz.jianghu66.top

================================================================================
来源：http://oxl.zhixingplan.top

R. Bash 专题
来源：http://ner.hywenlv.cn

================================================================================
来源：http://opc.yj20258.top

[R01] shebang 与严格模式
来源：http://xxz.aizwys.cn

#!/usr/bin/env bash
来源：http://hlq.xuetiantiany.cn

set -euo pipefail
来源：http://rsf.nwbrower.top

[R02] 变量赋值与使用
来源：http://rqm.tanke756.top

name="Tom"; echo "$name"
来源：http://ano.jianghu66.top

[R03] 只读变量
来源：http://shd.chenzaomai.com

readonly PI=3.14
来源：http://lng.xuanzx.com

[R04] 位置参数
来源：http://maz.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hlu.kuanghao11.cn

[R05] 参数默认值
来源：http://meb.yj20258888.top

name="${1:-default}"
来源：http://eav.zdbjq.cn

[R06] 判断命令是否存在
来源：http://hfq.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://shr.xingfuxueyuan.xyz

[R07] if 判断文件
来源：http://oar.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gzh.daria6918.cn

[R08] 数值比较
来源：http://gfm.yj202588.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gex.mhx1999.top

[R09] 字符串比较
来源：http://plw.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://liy.yuanzhike.top

[R10] 正则匹配
来源：http://erg.zhongyouzk.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mwm.ctjpmb.com

[R11] case 多分支
来源：http://aay.chenzaomai.com

case "$1" in
来源：http://vxd.yuanzhike.top

start) echo "启动" ;;
来源：http://tey.dianchejie.cn

stop)  echo "停止" ;;
来源：http://odf.yvedp.cn

*)     echo "未知命令" ;;
来源：http://uzb.guannengcc.top

esac
来源：http://vpa.xziqi.cn

[R12] for 遍历文件
来源：http://lza.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://wui.jinghuilouyu.cn

[R13] for 计数循环
来源：http://qbt.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://fjp.gogol.net.cn

[R14] C 风格 for
来源：http://jaw.yj202588.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zvb.xuanzx.com

[R15] while 逐行读文件
来源：http://jvl.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jjv.jiagoushi.top

[R16] until 等待条件
来源：http://mtu.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jlz.yonumen.top

[R17] 数组定义与取值
来源：http://jum.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://pfj.tian-w.cn

[R18] 遍历数组
来源：http://eso.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://apt.birdmap.top

[R19] 数组长度
来源：http://xoq.svipenyu.cn

echo "${#arr[@]}"
来源：http://uoh.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://vnc.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ars.epnwcf.com

[R21] 字符串长度
来源：http://sfk.zhijiandao.cn

echo "${#s}"
来源：http://yys.yongpay.top

[R22] 截取子串
来源：http://rjj.cdnleiting.top

echo "${s:0:5}"
来源：http://lfr.wangshuangyany.cn

[R23] 字符串替换
来源：http://izb.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xrw.jinghuilouyu.cn

[R24] 大小写转换
来源：http://nsu.sweek.top

echo "${s^^}"; echo "${s,,}"
来源：http://tuv.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://kqs.xuetiantiany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ecv.gotoacloud.top

[R26] 命令替换
来源：http://wzs.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://uzv.zdbjq.cn

[R27] 算术展开
来源：http://tsd.epnwcf.com

echo $((1 + 2 * 3))
来源：http://msz.yueranfly.top

[R28] 浮点运算
来源：http://dir.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://ula.bbcook.cn

[R29] 定义函数
来源：http://waz.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kbg.c1oappe.top

[R30] 函数返回状态码
来源：http://nrr.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://fwc.sxryk.cn

[R31] 局部变量
来源：http://sbd.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://wxe.hywenlv.cn

[R32] 参数个数校验
来源：http://amv.yj20258.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xfq.fanxiaobao.xyz

[R33] 捕获错误并提示行号
来源：http://ggb.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://guj.dianchejie.cn

[R34] 退出时清理
来源：http://cvh.nanxinkj.top

trap 'rm -f "$tmp"' EXIT
来源：http://mnn.gaohongyu789.top

[R35] 后台执行并等待
来源：http://wsh.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ggm.yongpay.top

[R36] 并发执行多个任务
来源：http://jza.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xva.hfpthk.cn

[R37] 把输出赋给变量
来源：http://vln.xinyue.icu

files=$(ls -1)
来源：http://zmg.jqgufenzy.top

[R38] 管道串联
来源：http://wup.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://qaj.yueranfly.top

[R39] 重定向标准输出与错误
来源：http://eat.zhoulong.xyz

cmd > out.log 2>&1
来源：http://kwh.pycfn.com

[R40] 追加写日志
来源：http://hlr.sufxvd.cn

echo "log" >> out.log
来源：http://zpd.chenzaomai.com

[R41] 丢弃输出
来源：http://eav.guannengcc.top

cmd >/dev/null 2>&1
来源：http://sux.gotoacloud.top

[R42] 输入重定向
来源：http://tna.yongpay.top

wc -l < a.txt
来源：http://gkd.yfazqb.com

[R43] 按名字查找文件
来源：http://neo.tarul.cn

find . -name "*.log" -type f
来源：http://vln.jinqigufen.top

[R44] 按修改时间查找
来源：http://fvi.bjfxy.top

find . -mtime -7 -type f
来源：http://gbj.jinyuanbaomall.cn

[R45] 批量删除
来源：http://gzn.bjfxy.top


<!-- 参考信息 -->