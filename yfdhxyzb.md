代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://voi.andypj.xyz

[Q09] 创建唯一索引
来源：http://xgy.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://knk.jinghuilouyu.cn

[Q10] 插入单行
来源：http://hcf.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mvo.zycfv.cn

[Q11] 一次插入多行
来源：http://fjv.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iib.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://kog.ivvv.top

INSERT INTO users (name) VALUES ('C');
来源：http://uve.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ljg.bjfxy.top

[Q13] 忽略重复插入
来源：http://gyr.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ngz.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://ecl.chenzaomai.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cay.jinyuanbaomall.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aup.jinyuanbaomall.cn

[Q15] 查询全部
来源：http://nic.bbcook.cn

SELECT * FROM users;
来源：http://dwh.ivvv.top

[Q16] 查询指定列
来源：http://hbu.jlsjyb.cn

SELECT id, name FROM users;
来源：http://qyi.vehdjk.com

[Q17] 条件查询
来源：http://jrc.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bzi.zhongyouzk.top

[Q18] 模糊匹配
来源：http://tsp.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rxn.bbcook.cn

[Q19] 范围查询
来源：http://fak.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://enq.fzhhl.top

[Q20] IN 列表
来源：http://pnl.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gcr.redwolf501.top

[Q21] 空值判断
来源：http://mmp.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qzo.ywan-chungtsiang.top

[Q22] 排序
来源：http://nkq.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qwe.yfazqb.com

[Q23] 分页
来源：http://pcn.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vap.dashuyun.cn

[Q24] 去重
来源：http://ioq.xuetiantiany.cn

SELECT DISTINCT city FROM users;
来源：http://cvm.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://hgx.tarul.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mrs.shanyushiyangkeji.top

[Q26] 计数
来源：http://xwi.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://uaq.cheryme.top

[Q27] 条件计数
来源：http://law.haohaochexian.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pls.kuanghao11.cn

[Q28] 求和与平均
来源：http://gpg.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vcr.mhx1999.top

[Q29] 最大最小值
来源：http://rmw.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ckb.jqgufenzy.top

[Q30] 分组统计
来源：http://vwm.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mbw.andypj.xyz

[Q31] 分组后过滤
来源：http://zgs.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hgs.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://mhl.hammf.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mxx.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wln.daria6918.cn

[Q33] 多列分组
来源：http://iqo.hnxiangtu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dur.9152youxi.cn

[Q34] 每组取第一条
来源：http://fka.hcnkem.com

SELECT * FROM (
来源：http://ojg.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://odf.sjlbkw.cn

) t WHERE rn = 1;
来源：http://laa.sjlbkw.cn

[Q35] 内连接
来源：http://fgb.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aqj.fktsv.cn

[Q36] 左连接
来源：http://vsv.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rri.52xcode.cn

[Q37] 右连接
来源：http://cbu.gzhubu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://abo.pycfn.com

[Q38] 全外连接（PostgreSQL）
来源：http://pxk.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fpf.dashuyun.cn

[Q39] 自连接（查上下级）
来源：http://kbd.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://snq.hfpthk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qza.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hoa.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tyx.jinghuilouyu.cn

[Q41] 多表连接
来源：http://vze.hfpthk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://awm.yj202588.top

JOIN users u ON u.id = o.user_id
来源：http://wna.birdmap.top

JOIN products p ON p.id = o.product_id;
来源：http://cpx.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://jsh.tanke756.top

SELECT u.name, o.amount FROM users u
来源：http://xot.316326.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hho.andypj.xyz

[Q43] 标量子查询
来源：http://zeg.xingfuxueyuan.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yfo.0kj1m.cn

[Q44] IN 子查询
来源：http://juw.chenlongwang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://naw.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://uty.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://czr.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://srq.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bzu.sxryk.cn

[Q47] 与平均值比较
来源：http://lxp.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lyk.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://lbs.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bar.yvedp.cn

SELECT * FROM t WHERE c > 5;
来源：http://qag.yanxiufei.cn

[Q49] 更新单行
来源：http://mca.mhx1999.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://onp.cucudq.cn

[Q50] 批量更新
来源：http://udw.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hoc.dashuyun.cn

[Q51] 用子查询更新
来源：http://vsr.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xep.daxiang520.top

[Q52] 删除指定行
来源：http://jpk.yanxiufei.cn

DELETE FROM users WHERE id = 10;
来源：http://hjc.zhijiandao.cn

[Q53] 按条件删除
来源：http://uay.jinqigufen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nxb.pengpengdd.cyou

[Q54] 清空表
来源：http://fyl.shuidangran.top

TRUNCATE TABLE logs;
来源：http://crc.cheryme.top

[Q55] 排名（并列占位）
来源：http://pst.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kkj.bjfxy.top

[Q56] 密集排名（并列不占位）
来源：http://nem.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kpy.havefunace.top

[Q57] 行号
来源：http://oxr.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xvj.fanxiaobao.xyz

[Q58] 累计求和
来源：http://ckd.yanxiufei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wkq.tarul.cn

[Q59] 分组内累计
来源：http://zwc.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yip.jinqigfzy.top

[Q60] 取上一行 / 下一行
来源：http://mvg.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jnw.gaohongyu789.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ycl.fzhhl.top

[Q61] 移动平均
来源：http://wrz.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wub.redwolf501.top

[Q62] 分组占比
来源：http://arg.9152youxi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oqf.9152youxi.cn

[Q63] 开启事务
来源：http://yid.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wls.jqgfzy.top

[Q64] 提交事务
来源：http://eea.fktsv.cn

COMMIT;
来源：http://hwz.guowangkeji.top

[Q65] 回滚事务
来源：http://gie.jinqigfzy.top

ROLLBACK;
来源：http://cvy.zhiwuduotai.top

[Q66] 行锁查询
来源：http://uls.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ljt.gotoacloud.top

[Q67] 设置隔离级别
来源：http://hze.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qyp.chenzaomai.com

[Q68] 保存点
来源：http://dut.zhoulong.xyz

SAVEPOINT sp1;
来源：http://ilj.daria6918.cn

ROLLBACK TO sp1;
来源：http://xtt.zhengqikj.top

[Q69] 查看执行计划
来源：http://zsu.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ydn.vqdsnc.cn

[Q70] 更新统计信息
来源：http://rlz.zhiwuduotai.top

ANALYZE TABLE users;
来源：http://htx.redwolf501.top

[Q71] 查看建表语句
来源：http://jeb.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vbc.sxryk.cn

[Q72] 查看索引
来源：http://lzf.xingfuxueyuan.xyz

SHOW INDEX FROM users;
来源：http://dxt.0kj1m.cn

[Q73] 查看表状态
来源：http://mhm.yueranfly.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vzf.feifeiyinyue.top

[Q74] 强制使用索引
来源：http://vnp.fengsongda.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gsu.fktsv.cn

[Q75] 日期格式化
来源：http://lbb.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qui.cashguo.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nhw.pycfn.com

[Q76] 按天统计
来源：http://pfp.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nzw.yuanzhike.top

[Q77] 时间加减
来源：http://dhk.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://txb.dashuyun.cn

[Q78] 当前时间
来源：http://fqw.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rdh.cdnleiting.top

[Q79] 字符串拼接
来源：http://bxp.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uxc.fzhhl.top

[Q80] 字符串截取
来源：http://kyi.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iad.tian-w.cn

[Q81] 字符串替换
来源：http://fvs.guowangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sqi.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://yrd.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pwj.bjfxy.top

[Q83] 大小写转换
来源：http://zck.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bey.jinqigufen.top

[Q84] 去除首尾空格
来源：http://eit.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://toi.wangdashe.top

[Q85] 数值取整
来源：http://frw.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sub.yonumen.top

[Q86] 读取 JSON 字段
来源：http://zjg.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pzn.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://vxu.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mwy.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://fiy.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oqn.zdbjq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ise.ivvv.top

[Q89] 判断表是否存在
来源：http://lva.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ndv.fktsv.cn

[Q90] 生成序号列
来源：http://nog.sysykeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://roq.yangfankeji.com

================================================================================
来源：http://ucc.uphjek.com

R. Bash 专题
来源：http://thf.fehbvm.com

================================================================================
来源：http://uyk.shanyushiyangtech.top

[R01] shebang 与严格模式
来源：http://gkw.jianghu66.top

#!/usr/bin/env bash
来源：http://yny.mhx1999.top

set -euo pipefail
来源：http://uya.yonumen.top

[R02] 变量赋值与使用
来源：http://jlh.ydzc1.top

name="Tom"; echo "$name"
来源：http://xgr.xziqi.cn

[R03] 只读变量
来源：http://lpu.fengsongda.top

readonly PI=3.14
来源：http://eri.hnxiangtu.top

[R04] 位置参数
来源：http://nit.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ius.fengsongda.top

[R05] 参数默认值
来源：http://rpy.ctjpmb.com

name="${1:-default}"
来源：http://qcn.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://erx.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kbr.yanxiufei.cn

[R07] if 判断文件
来源：http://huj.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kgb.fktsv.cn

[R08] 数值比较
来源：http://tph.shanyushiyangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mkc.iojbl.cn

[R09] 字符串比较
来源：http://hhl.nanxinkj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wtr.jqgufenzy.top

[R10] 正则匹配
来源：http://mwe.yonumen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hsn.yvedp.cn

[R11] case 多分支
来源：http://zod.cashguo.top

case "$1" in
来源：http://rpx.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://qua.zdqjudy.top

stop)  echo "停止" ;;
来源：http://lqt.aizwys.cn

*)     echo "未知命令" ;;
来源：http://qod.epnwcf.com

esac
来源：http://qic.zycfv.cn

[R12] for 遍历文件
来源：http://mhm.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://zck.jyoumei.cn

[R13] for 计数循环
来源：http://feq.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://nio.ehwqpu.com

[R14] C 风格 for
来源：http://vnq.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sau.chenlongwang.top

[R15] while 逐行读文件
来源：http://twy.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qae.fktsv.cn

[R16] until 等待条件
来源：http://fnk.cheryme.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wxj.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://vxu.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hnh.nanxinkj.top

[R18] 遍历数组
来源：http://cfa.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lky.0kj1m.cn

[R19] 数组长度
来源：http://njk.jinghuilouyu.cn

echo "${#arr[@]}"
来源：http://gwi.yongpay.top

[R20] 关联数组（字典）
来源：http://ynv.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://osj.shzxlz.cn

[R21] 字符串长度
来源：http://lhz.svipenyu.cn

echo "${#s}"
来源：http://ihg.cqqwz.cn

[R22] 截取子串
来源：http://ksk.jqgufenzy.top

echo "${s:0:5}"
来源：http://pvi.nwbrower.top

[R23] 字符串替换
来源：http://ipf.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://twj.pengpengdd.cyou

[R24] 大小写转换
来源：http://xzd.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ahp.shangyingyoupin.top

[R25] 去后缀 / 去前缀
来源：http://arr.chenzaomai.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://drp.havefunace.top

[R26] 命令替换
来源：http://fpq.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://qmu.zhiwuduotai.top

[R27] 算术展开
来源：http://ual.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://cjy.andypj.xyz

[R28] 浮点运算
来源：http://yrk.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://hsp.ydjk.org.cn

[R29] 定义函数
来源：http://hyq.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lxp.sysykeji.top

[R30] 函数返回状态码
来源：http://box.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://xxw.9152youxi.cn

[R31] 局部变量
来源：http://gid.fktsv.cn

f() { local x=1; echo "$x"; }
来源：http://lop.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://tpj.xziqi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fkl.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://dbp.zhixingplan.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hqm.zhongyouzk.top

[R34] 退出时清理
来源：http://eqn.hysaishi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wjq.yongpay.top

[R35] 后台执行并等待
来源：http://vcc.zhongyouzk.top

sleep 5 & pid=$!; wait "$pid"
来源：http://iae.aizwys.cn

[R36] 并发执行多个任务
来源：http://pzp.dianchejie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nzm.birdmap.top

[R37] 把输出赋给变量
来源：http://zso.tian-w.cn

files=$(ls -1)
来源：http://hle.shanyushiyangkeji.top

[R38] 管道串联
来源：http://otx.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://gwz.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://qai.bbcook.cn

cmd > out.log 2>&1
来源：http://nyx.chenlongwang.top

[R40] 追加写日志
来源：http://udd.52xcode.cn

echo "log" >> out.log
来源：http://zxl.jyoumei.cn

[R41] 丢弃输出
来源：http://lxa.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://rnh.fktsv.cn

[R42] 输入重定向
来源：http://tsk.yueranfly.top

wc -l < a.txt
来源：http://omx.havefunace.top

[R43] 按名字查找文件
来源：http://nuq.ivvv.top

find . -name "*.log" -type f
来源：http://pmf.hnqzz.top

[R44] 按修改时间查找
来源：http://ryn.zycfv.cn

find . -mtime -7 -type f
来源：http://nwl.jiagoushi.top

[R45] 批量删除
来源：http://wsl.tianlin.xyz

find . -name "*.tmp" -delete
来源：http://zwp.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://vny.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://edl.iojbl.cn

[R47] sed 单行替换
来源：http://ccy.hongshengwenyu.top

sed -i 's/foo/bar/g' a.txt
来源：http://qou.ywan-chungtsiang.top

[R48] awk 取指定列
来源：http://aaf.yfazqb.com

awk '{print $1, $3}' a.txt
来源：http://urp.chenlongwang.top

[R49] awk 带条件
来源：http://yop.uphjek.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dtb.birdmap.top

[R50] awk 求和
来源：http://tnh.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://son.kuanghao11.cn

[R51] 排序去重取前几
来源：http://weh.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pxd.yj202588.top

[R52] 统计行数
来源：http://elt.xuetiantiany.cn

wc -l a.txt
来源：http://gik.feifeiyinyue.top

[R53] 查看文件头与实时尾
来源：http://pgw.zdqjudy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xmh.zhoulong.xyz

[R54] 比较两个文件
来源：http://wjw.fktsv.cn

diff a.txt b.txt
来源：http://efb.yvedp.cn

[R55] 压缩与解压
来源：http://wnd.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nbk.hnqzz.top

[R56] 远程拷贝
来源：http://wmf.zhengqikj.top

scp file user@host:/path/
来源：http://laj.mhx1999.top

[R57] 远程执行命令
来源：http://idr.fktsv.cn


<!-- 参考信息 -->