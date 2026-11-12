代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://msh.ivvv.top

[Q07] 删除表
来源：http://nxg.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://gyj.jqgufenzy.top

[Q08] 创建普通索引
来源：http://szw.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mnl.tianlin.xyz

[Q09] 创建唯一索引
来源：http://yks.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://krh.cashguo.top

[Q10] 插入单行
来源：http://izl.52xcode.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kta.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://nfs.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dcs.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://pzk.ehwqpu.com

INSERT INTO users (name) VALUES ('C');
来源：http://wmi.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uqj.gotoacloud.top

[Q13] 忽略重复插入
来源：http://odj.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rjs.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://ujk.jinghuilouyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ojy.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://apn.aibaodan.cn

[Q15] 查询全部
来源：http://rob.jiagoushi.top

SELECT * FROM users;
来源：http://fvc.yuxming.cn

[Q16] 查询指定列
来源：http://xdr.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://gpe.mhx1999.top

[Q17] 条件查询
来源：http://hry.jinghuilouyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://drl.sweek.top

[Q18] 模糊匹配
来源：http://kul.hesvh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zqh.ywan-chungtsiang.top

[Q19] 范围查询
来源：http://bwt.fzhhl.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wqn.haohaochexian.top

[Q20] IN 列表
来源：http://qmg.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://krt.ivvv.top

[Q21] 空值判断
来源：http://ymw.chenlongwang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vsx.gogol.net.cn

[Q22] 排序
来源：http://cch.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pbc.vqdsnc.cn

[Q23] 分页
来源：http://rqc.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nbf.kuanghao11.cn

[Q24] 去重
来源：http://ery.yonumen.top

SELECT DISTINCT city FROM users;
来源：http://xxu.cheryme.top

[Q25] 只取前 N 条
来源：http://xcp.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bsj.yongpay.top

[Q26] 计数
来源：http://ael.hcnkem.com

SELECT COUNT(*) FROM users;
来源：http://tll.yuanzhike.top

[Q27] 条件计数
来源：http://vdl.fehbvm.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fvc.aizwys.cn

[Q28] 求和与平均
来源：http://utu.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ouq.gaohongyu789.top

[Q29] 最大最小值
来源：http://xtj.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://jzv.hcnkem.com

[Q30] 分组统计
来源：http://rai.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gwo.yongpay.top

[Q31] 分组后过滤
来源：http://mdn.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kmp.zhongyouzk.top

[Q32] 分组拼接字符串
来源：http://kil.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ckz.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bdf.c1oappe.top

[Q33] 多列分组
来源：http://kgp.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cwk.chenlongwang.top

[Q34] 每组取第一条
来源：http://hkz.dianchejie.cn

SELECT * FROM (
来源：http://vsy.52xcode.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aqy.yfazqb.com

) t WHERE rn = 1;
来源：http://ats.meibo888.top

[Q35] 内连接
来源：http://uop.ivvv.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yzd.svipenyu.cn

[Q36] 左连接
来源：http://rzs.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ses.ivvv.top

[Q37] 右连接
来源：http://mim.zhoulong.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hzh.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://fqj.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tjd.yongpay.top

[Q39] 自连接（查上下级）
来源：http://yhn.yj20258888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lfv.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mrd.chenlongwang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cpo.shanyushiyangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wqk.jqgufenzy.top

[Q41] 多表连接
来源：http://ybk.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ria.shanyushiyangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://mgp.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://ejd.jqgfzy.top

[Q42] 连接条件附加过滤
来源：http://tnk.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u
来源：http://hle.nanxinkj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://edn.bjfxy.top

[Q43] 标量子查询
来源：http://jqr.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kcy.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://lsj.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lmy.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://jhh.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ubs.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vgr.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fls.jqgufenzy.top

[Q47] 与平均值比较
来源：http://juu.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zqh.9152youxi.cn

[Q48] CTE 公用表表达式
来源：http://stu.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yrf.shanyushiyangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://kph.hcnkem.com

[Q49] 更新单行
来源：http://odc.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lxy.zhijiandao.cn

[Q50] 批量更新
来源：http://uwk.birdmap.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vee.uphjek.com

[Q51] 用子查询更新
来源：http://nir.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qcn.gogol.net.cn

[Q52] 删除指定行
来源：http://qvo.jianghu66.top

DELETE FROM users WHERE id = 10;
来源：http://aoq.yongpay.top

[Q53] 按条件删除
来源：http://rru.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vgz.quarkkingdee.top

[Q54] 清空表
来源：http://pdy.redwolf501.top

TRUNCATE TABLE logs;
来源：http://oii.fzhhl.top

[Q55] 排名（并列占位）
来源：http://idp.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://osm.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://ncz.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ubu.jqgfzy.top

[Q57] 行号
来源：http://umh.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kpt.aizwys.cn

[Q58] 累计求和
来源：http://omz.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lib.316326.xyz

[Q59] 分组内累计
来源：http://epo.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wvx.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://qpq.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pde.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qew.andypj.xyz

[Q61] 移动平均
来源：http://vxm.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cas.pengpengdd.cyou

[Q62] 分组占比
来源：http://zdp.meibo888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cgi.zhijiandao.cn

[Q63] 开启事务
来源：http://pov.redwolf501.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kha.yj20258888.top

[Q64] 提交事务
来源：http://cak.jinqigfzy.top

COMMIT;
来源：http://ibs.yangfankeji.com

[Q65] 回滚事务
来源：http://vrm.yvedp.cn

ROLLBACK;
来源：http://wiq.aizwys.cn

[Q66] 行锁查询
来源：http://unm.kuanghao11.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vpk.vehdjk.com

[Q67] 设置隔离级别
来源：http://fnq.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zch.tian-w.cn

[Q68] 保存点
来源：http://wlw.andypj.xyz

SAVEPOINT sp1;
来源：http://rkm.tian-w.cn

ROLLBACK TO sp1;
来源：http://ijw.xingfuxueyuan.xyz

[Q69] 查看执行计划
来源：http://pvk.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vha.bjfxy.top

[Q70] 更新统计信息
来源：http://vvv.yanxiufei.cn

ANALYZE TABLE users;
来源：http://cxn.zdqjudy.top

[Q71] 查看建表语句
来源：http://guy.aibaodan.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ays.fehbvm.com

[Q72] 查看索引
来源：http://zwh.vqdsnc.cn

SHOW INDEX FROM users;
来源：http://mfo.yonumen.top

[Q73] 查看表状态
来源：http://ubz.zhijiandao.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zxs.hnxiangtu.top

[Q74] 强制使用索引
来源：http://spe.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gze.dashuyun.cn

[Q75] 日期格式化
来源：http://kkj.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vpn.xylfe.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://khv.tarul.cn

[Q76] 按天统计
来源：http://vpv.hammf.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://avp.xuanzx.com

[Q77] 时间加减
来源：http://eek.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qmx.meibo888.top

[Q78] 当前时间
来源：http://ssn.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qwo.ivvv.top

[Q79] 字符串拼接
来源：http://dlq.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ndp.hesvh.cn

[Q80] 字符串截取
来源：http://ect.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gue.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://ybk.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iip.316326.xyz

[Q82] 字符长度与字节长度
来源：http://kfy.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wvd.ydjk.org.cn

[Q83] 大小写转换
来源：http://stk.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pvf.xziqi.cn

[Q84] 去除首尾空格
来源：http://pgw.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://uil.yueranfly.top

[Q85] 数值取整
来源：http://xxc.c1oappe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zvw.havefunace.top

[Q86] 读取 JSON 字段
来源：http://err.chenlongwang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rib.cqqwz.cn

[Q87] JSON 字段做条件
来源：http://tjj.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kgy.yfazqb.com

[Q88] 行转列（条件聚合）
来源：http://oft.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sqe.dianchejie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ucj.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://zvj.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rez.guannengcc.top

[Q90] 生成序号列
来源：http://ged.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://quj.dianchejie.cn

================================================================================
来源：http://uva.cheryme.top

R. Bash 专题
来源：http://xdg.yj202588.top

================================================================================
来源：http://mmx.fzhhl.top

[R01] shebang 与严格模式
来源：http://pnr.yj202588.top

#!/usr/bin/env bash
来源：http://hnq.jianghu66.top

set -euo pipefail
来源：http://uvr.fehbvm.com

[R02] 变量赋值与使用
来源：http://rul.daxiang520.top

name="Tom"; echo "$name"
来源：http://leo.sxryk.cn

[R03] 只读变量
来源：http://dld.ctjpmb.com

readonly PI=3.14
来源：http://ikv.yj20258888.top

[R04] 位置参数
来源：http://uzb.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cww.jyoumei.cn

[R05] 参数默认值
来源：http://dlv.mhx1999.top

name="${1:-default}"
来源：http://mlv.aibaodan.cn

[R06] 判断命令是否存在
来源：http://nrx.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pzb.fzhhl.top

[R07] if 判断文件
来源：http://wkj.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qim.ctjpmb.com

[R08] 数值比较
来源：http://zgy.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://syj.chenlongwang.top

[R09] 字符串比较
来源：http://vbl.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gcy.sweek.top

[R10] 正则匹配
来源：http://tky.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rnk.jianghu66.top

[R11] case 多分支
来源：http://yam.jianghu66.top

case "$1" in
来源：http://pul.daria6918.cn

start) echo "启动" ;;
来源：http://piy.fzhhl.top

stop)  echo "停止" ;;
来源：http://yjh.xingfuxueyuan.xyz

*)     echo "未知命令" ;;
来源：http://kyd.sjlbkw.cn

esac
来源：http://sgl.jianghu66.top

[R12] for 遍历文件
来源：http://een.jqgfzy.top

for f in *.txt; do echo "$f"; done
来源：http://htd.mhx1999.top

[R13] for 计数循环
来源：http://inl.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://adu.sysykeji.top

[R14] C 风格 for
来源：http://jwx.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ihh.meibo888.top

[R15] while 逐行读文件
来源：http://cue.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xgd.zhijiandao.cn

[R16] until 等待条件
来源：http://wrc.chenzaomai.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tkl.gogol.net.cn

[R17] 数组定义与取值
来源：http://vjs.feifeiyinyue.top

arr=(a b c); echo "${arr[0]}"
来源：http://qgo.zdbjq.cn

[R18] 遍历数组
来源：http://oyh.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://afy.ywan-chungtsiang.top

[R19] 数组长度
来源：http://zad.ctjpmb.com

echo "${#arr[@]}"
来源：http://cgu.sxryk.cn

[R20] 关联数组（字典）
来源：http://hdv.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wna.zycfv.cn

[R21] 字符串长度
来源：http://wqe.jqgufenzy.top

echo "${#s}"
来源：http://skt.zhixingplan.top

[R22] 截取子串
来源：http://fpv.fehbvm.com

echo "${s:0:5}"
来源：http://xbi.sufxvd.cn

[R23] 字符串替换
来源：http://szm.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lcf.zhengqikj.top

[R24] 大小写转换
来源：http://jws.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://jaw.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://epv.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cxh.yuxming.cn

[R26] 命令替换
来源：http://gji.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://sdy.aibaodan.cn

[R27] 算术展开
来源：http://vvt.dianchejie.cn

echo $((1 + 2 * 3))
来源：http://bjy.316326.xyz

[R28] 浮点运算
来源：http://mhp.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://ena.dianchejie.cn

[R29] 定义函数
来源：http://yku.ctjpmb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dzu.redwolf501.top

[R30] 函数返回状态码
来源：http://djw.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://jtk.wangdashe.top

[R31] 局部变量
来源：http://npg.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://nde.ppjwa.cn

[R32] 参数个数校验
来源：http://lhi.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lfn.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://hro.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sed.vqdsnc.cn

[R34] 退出时清理
来源：http://paj.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://scm.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://jje.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vzp.gogol.net.cn

[R36] 并发执行多个任务
来源：http://mjd.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cqg.sjlbkw.cn

[R37] 把输出赋给变量
来源：http://zlv.jiagoushi.top

files=$(ls -1)
来源：http://dfc.haohaochexian.top

[R38] 管道串联
来源：http://fip.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://rem.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://ayj.gaohongyu789.top

cmd > out.log 2>&1
来源：http://jug.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://mpe.zhongyouzk.top

echo "log" >> out.log
来源：http://jmj.ppjwa.cn

[R41] 丢弃输出
来源：http://qev.feifeiyinyue.top

cmd >/dev/null 2>&1
来源：http://aaw.yangfankeji.com

[R42] 输入重定向
来源：http://bvp.shanyushiyangtech.top

wc -l < a.txt
来源：http://zen.bjfxy.top

[R43] 按名字查找文件
来源：http://gcb.tianlin.xyz

find . -name "*.log" -type f
来源：http://maw.dianchejie.cn

[R44] 按修改时间查找
来源：http://vor.nanxuanxn.top

find . -mtime -7 -type f
来源：http://ogc.hnxiangtu.top

[R45] 批量删除
来源：http://nrd.fktsv.cn

find . -name "*.tmp" -delete
来源：http://apo.gzhubu.top

[R46] 递归替换文件内容
来源：http://rxk.ctjpmb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gyo.haohaochexian.top

[R47] sed 单行替换
来源：http://dvs.smart0.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://dfg.yfazqb.com

[R48] awk 取指定列
来源：http://szq.ydjk.org.cn

awk '{print $1, $3}' a.txt
来源：http://uwr.hnqzz.top

[R49] awk 带条件
来源：http://hkp.jyoumei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ofh.yangfankeji.com

[R50] awk 求和
来源：http://ijq.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://ubc.aibaodan.cn

[R51] 排序去重取前几
来源：http://cuv.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mep.ywan-chungtsiang.top

[R52] 统计行数
来源：http://erk.zhixingplan.top

wc -l a.txt
来源：http://xqp.wangdashe.top

[R53] 查看文件头与实时尾
来源：http://fua.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ktx.mhx1999.top

[R54] 比较两个文件
来源：http://frk.bjfxy.top

diff a.txt b.txt
来源：http://sxy.hesvh.cn

[R55] 压缩与解压
来源：http://ave.ppjwa.cn


<!-- 参考信息 -->