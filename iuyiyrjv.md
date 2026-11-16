代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://len.daxiang520.top

[Q07] 删除表
来源：http://ycl.yanxiufei.cn

DROP TABLE IF EXISTS orders;
来源：http://jeg.fehbvm.com

[Q08] 创建普通索引
来源：http://ijm.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gsw.fktsv.cn

[Q09] 创建唯一索引
来源：http://vzq.svipenyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dtl.cheryme.top

[Q10] 插入单行
来源：http://bdh.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tim.zhixingplan.top

[Q11] 一次插入多行
来源：http://xzm.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ohx.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://oea.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://mbw.nanxuanxn.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://heh.yueranfly.top

[Q13] 忽略重复插入
来源：http://xoa.zhixingplan.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uho.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://lkk.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://knq.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qpj.zhengqikj.top

[Q15] 查询全部
来源：http://ump.cqqwz.cn

SELECT * FROM users;
来源：http://ltk.9152youxi.cn

[Q16] 查询指定列
来源：http://ghv.jianghu66.top

SELECT id, name FROM users;
来源：http://pvx.316326.xyz

[Q17] 条件查询
来源：http://jqo.jyoumei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eiw.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://pdu.hywenlv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uhv.sweek.top

[Q19] 范围查询
来源：http://iyn.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pfa.xinyue.icu

[Q20] IN 列表
来源：http://qat.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jwq.hcnkem.com

[Q21] 空值判断
来源：http://jtj.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uxu.nanxuanxn.top

[Q22] 排序
来源：http://fax.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://msd.jinqigufen.top

[Q23] 分页
来源：http://vok.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ozj.sxryk.cn

[Q24] 去重
来源：http://sob.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://nkb.yangfankeji.com

[Q25] 只取前 N 条
来源：http://xbg.vqdsnc.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hij.0kj1m.cn

[Q26] 计数
来源：http://kyt.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://vkd.xinyue.icu

[Q27] 条件计数
来源：http://aht.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vus.sxryk.cn

[Q28] 求和与平均
来源：http://mss.jinqigufen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wtk.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://woi.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://efw.sxryk.cn

[Q30] 分组统计
来源：http://kwk.zhoulong.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vfr.jianghu66.top

[Q31] 分组后过滤
来源：http://ksy.birdmap.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vhy.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://hut.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uae.zhengqikj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ruk.fktsv.cn

[Q33] 多列分组
来源：http://suh.jyoumei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gub.sweek.top

[Q34] 每组取第一条
来源：http://sqr.sjlbkw.cn

SELECT * FROM (
来源：http://wno.kuanghao11.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cux.hnqzz.top

) t WHERE rn = 1;
来源：http://wgy.jianghu66.top

[Q35] 内连接
来源：http://gyc.bjfxy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lxz.xylfe.cn

[Q36] 左连接
来源：http://hqn.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qih.yvedp.cn

[Q37] 右连接
来源：http://nhw.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hnw.tian-w.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uym.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nlm.xuanzx.com

[Q39] 自连接（查上下级）
来源：http://crm.hysaishi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://osi.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jzt.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://egp.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fpe.jiagoushi.top

[Q41] 多表连接
来源：http://wzt.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jwz.pengpengdd.cyou

JOIN users u ON u.id = o.user_id
来源：http://vpf.daxiang520.top

JOIN products p ON p.id = o.product_id;
来源：http://yrm.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://oyc.zhengqikj.top

SELECT u.name, o.amount FROM users u
来源：http://bkb.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uxi.fengsongda.top

[Q43] 标量子查询
来源：http://qvt.tian-w.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cbx.tianlin.xyz

[Q44] IN 子查询
来源：http://ddd.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ggq.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://uha.c1oappe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cnp.hnxiangtu.top

[Q46] NOT EXISTS 判断不存在
来源：http://glz.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gsc.ybcxt.top

[Q47] 与平均值比较
来源：http://rko.wangshuangyany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gac.sxryk.cn

[Q48] CTE 公用表表达式
来源：http://gxj.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://enp.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://bgl.xinyue.icu

[Q49] 更新单行
来源：http://xyk.jqgfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bap.ivvv.top

[Q50] 批量更新
来源：http://gvv.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ixh.nanxinkj.top

[Q51] 用子查询更新
来源：http://ewm.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rxy.xinyue.icu

[Q52] 删除指定行
来源：http://yem.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://tpx.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://btu.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rar.fanxiaobao.xyz

[Q54] 清空表
来源：http://prh.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://ybj.pengpengdd.cyou

[Q55] 排名（并列占位）
来源：http://dis.havefunace.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vjq.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://yhf.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ljd.gogol.net.cn

[Q57] 行号
来源：http://qxm.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qlp.nanxuanxn.top

[Q58] 累计求和
来源：http://ket.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nss.epnwcf.com

[Q59] 分组内累计
来源：http://rud.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ogn.tarul.cn

[Q60] 取上一行 / 下一行
来源：http://txr.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://its.yuanzhike.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://weu.sjlbkw.cn

[Q61] 移动平均
来源：http://uam.aizwys.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ywv.fanxiaobao.xyz

[Q62] 分组占比
来源：http://qxj.daria6918.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qic.xuanzx.com

[Q63] 开启事务
来源：http://lcd.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ufx.gaohongyu789.top

[Q64] 提交事务
来源：http://qsf.9152youxi.cn

COMMIT;
来源：http://lsc.zdqjudy.top

[Q65] 回滚事务
来源：http://nzv.xylfe.cn

ROLLBACK;
来源：http://rsc.haohaochexian.top

[Q66] 行锁查询
来源：http://sho.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yqm.fzhhl.top

[Q67] 设置隔离级别
来源：http://yaj.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bwt.sxryk.cn

[Q68] 保存点
来源：http://eac.hywenlv.cn

SAVEPOINT sp1;
来源：http://csx.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://rja.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://djl.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tdk.vqdsnc.cn

[Q70] 更新统计信息
来源：http://ryl.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://nny.andypj.xyz

[Q71] 查看建表语句
来源：http://ibd.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pjs.quarkkingdee.top

[Q72] 查看索引
来源：http://gyo.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://kzc.bbcook.cn

[Q73] 查看表状态
来源：http://lbc.fehbvm.com

SHOW TABLE STATUS LIKE 'users';
来源：http://mcd.xinyue.icu

[Q74] 强制使用索引
来源：http://xob.52xcode.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rue.chenlongwang.top

[Q75] 日期格式化
来源：http://lku.quarkkingdee.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pie.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pgt.cashguo.top

[Q76] 按天统计
来源：http://kca.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pfp.316326.xyz

[Q77] 时间加减
来源：http://xob.tianlin.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qyb.pengpengdd.cyou

[Q78] 当前时间
来源：http://rwt.chenzaomai.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pte.xziqi.cn

[Q79] 字符串拼接
来源：http://ajh.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qgx.hcnkem.com

[Q80] 字符串截取
来源：http://wuj.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nmr.meibo888.top

[Q81] 字符串替换
来源：http://zfb.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://coq.cashguo.top

[Q82] 字符长度与字节长度
来源：http://knk.yuanzhike.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cud.hongshengwenyu.top

[Q83] 大小写转换
来源：http://cfj.nanxinkj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://prj.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://fci.52xcode.cn

SELECT TRIM(name) FROM users;
来源：http://pxm.yuanzhike.top

[Q85] 数值取整
来源：http://rdd.chenzaomai.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iht.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://nbp.yueranfly.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bta.nwbrower.top

[Q87] JSON 字段做条件
来源：http://bpd.hammf.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fgk.shanyushiyangkeji.top

[Q88] 行转列（条件聚合）
来源：http://vig.yangfankeji.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bpu.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://plk.shanyushiyangkeji.top

[Q89] 判断表是否存在
来源：http://rne.ehwqpu.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ayc.pycfn.com

[Q90] 生成序号列
来源：http://gsc.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lvd.chenlongwang.top

================================================================================
来源：http://iwz.zhoulong.xyz

R. Bash 专题
来源：http://xcb.redwolf501.top

================================================================================
来源：http://cvk.sweek.top

[R01] shebang 与严格模式
来源：http://zow.jqgfzy.top

#!/usr/bin/env bash
来源：http://ezd.jyoumei.cn

set -euo pipefail
来源：http://lxs.andypj.xyz

[R02] 变量赋值与使用
来源：http://edj.tian-w.cn

name="Tom"; echo "$name"
来源：http://evz.ydzc1.top

[R03] 只读变量
来源：http://dre.quarkkingdee.top

readonly PI=3.14
来源：http://yjl.dianchejie.cn

[R04] 位置参数
来源：http://cdk.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kjk.vqdsnc.cn

[R05] 参数默认值
来源：http://adq.zhixingplan.top

name="${1:-default}"
来源：http://bbo.ydzc1.top

[R06] 判断命令是否存在
来源：http://ypt.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ubs.shuidangran.top

[R07] if 判断文件
来源：http://bhj.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qbw.c1oappe.top

[R08] 数值比较
来源：http://btd.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://euu.yj20258888.top

[R09] 字符串比较
来源：http://aic.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jgh.gaohongyu789.top

[R10] 正则匹配
来源：http://lmw.yueranfly.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vva.guannengcc.top

[R11] case 多分支
来源：http://uhm.hongshengwenyu.top

case "$1" in
来源：http://kyt.zdbjq.cn

start) echo "启动" ;;
来源：http://cdg.sweek.top

stop)  echo "停止" ;;
来源：http://vlg.hnqzz.top

*)     echo "未知命令" ;;
来源：http://uud.jinyuanbaomall.cn

esac
来源：http://azv.gzhubu.top

[R12] for 遍历文件
来源：http://bsc.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://gmx.fengsongda.top

[R13] for 计数循环
来源：http://squ.hnqzz.top

for i in {1..10}; do echo "$i"; done
来源：http://kij.jinqigfzy.top

[R14] C 风格 for
来源：http://juv.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://keh.gotoacloud.top

[R15] while 逐行读文件
来源：http://xnw.ywan-chungtsiang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zxu.yfazqb.com

[R16] until 等待条件
来源：http://zjh.gaohongyu789.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qah.fzhhl.top

[R17] 数组定义与取值
来源：http://wld.quarkkingdee.top

arr=(a b c); echo "${arr[0]}"
来源：http://fek.ydjk.org.cn

[R18] 遍历数组
来源：http://bao.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://seu.pycfn.com

[R19] 数组长度
来源：http://pbu.hesvh.cn

echo "${#arr[@]}"
来源：http://mtm.smart0.xyz

[R20] 关联数组（字典）
来源：http://ecy.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tyt.yfazqb.com

[R21] 字符串长度
来源：http://bpd.zhoulong.xyz

echo "${#s}"
来源：http://jcw.hnqzz.top

[R22] 截取子串
来源：http://uyy.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://ihl.ppjwa.cn

[R23] 字符串替换
来源：http://xrl.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uep.zhoulong.xyz

[R24] 大小写转换
来源：http://hpc.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://efi.jinyuanbaomall.cn

[R25] 去后缀 / 去前缀
来源：http://ela.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://lhl.birdmap.top

[R26] 命令替换
来源：http://uxm.ydjk.org.cn

now=$(date +%F); echo "$now"
来源：http://xrv.jianghu66.top

[R27] 算术展开
来源：http://grw.yueranfly.top

echo $((1 + 2 * 3))
来源：http://sfx.yvedp.cn

[R28] 浮点运算
来源：http://rwk.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://khr.vqdsnc.cn

[R29] 定义函数
来源：http://erc.shuidangran.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oyn.zhongyouzk.top

[R30] 函数返回状态码
来源：http://lnv.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://eci.fanxiaobao.xyz

[R31] 局部变量
来源：http://qqr.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://jwf.yj202588.top

[R32] 参数个数校验
来源：http://fhs.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hli.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://juz.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qfd.ppjwa.cn

[R34] 退出时清理
来源：http://afp.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cur.tanke756.top

[R35] 后台执行并等待
来源：http://rhj.yvedp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hcg.xinyue.icu

[R36] 并发执行多个任务
来源：http://vtm.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vpo.xziqi.cn

[R37] 把输出赋给变量
来源：http://erf.shangyingyoupin.top

files=$(ls -1)
来源：http://jde.hywenlv.cn

[R38] 管道串联
来源：http://bba.hcnkem.com

cat a.txt | grep -i error | wc -l
来源：http://cah.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://wwy.guannengcc.top

cmd > out.log 2>&1
来源：http://sgt.kuanghao11.cn

[R40] 追加写日志
来源：http://qrq.yangfankeji.com

echo "log" >> out.log
来源：http://oki.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://ppx.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://kis.zhongyouzk.top

[R42] 输入重定向
来源：http://acb.zhiwuduotai.top

wc -l < a.txt
来源：http://wxy.cashguo.top

[R43] 按名字查找文件
来源：http://nch.sufxvd.cn

find . -name "*.log" -type f
来源：http://lew.nanxinkj.top

[R44] 按修改时间查找
来源：http://ydg.yueranfly.top

find . -mtime -7 -type f
来源：http://aet.guannengcc.top

[R45] 批量删除
来源：http://zgp.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://sst.xuetiantiany.cn

[R46] 递归替换文件内容
来源：http://nau.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://skc.zhengqikj.top

[R47] sed 单行替换
来源：http://ysa.cheryme.top

sed -i 's/foo/bar/g' a.txt
来源：http://kfl.fzhhl.top

[R48] awk 取指定列
来源：http://awv.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://vzb.cheryme.top

[R49] awk 带条件
来源：http://cos.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tix.cheryme.top

[R50] awk 求和
来源：http://rso.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://mvw.chenlongwang.top

[R51] 排序去重取前几
来源：http://dxp.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://phc.ivvv.top

[R52] 统计行数
来源：http://uhl.daxiang520.top

wc -l a.txt
来源：http://slt.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://fzq.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dvz.hnqzz.top

[R54] 比较两个文件
来源：http://kcd.xylfe.cn

diff a.txt b.txt
来源：http://rth.shuidangran.top

[R55] 压缩与解压
来源：http://gjt.nanxuanxn.top


<!-- 参考信息 -->