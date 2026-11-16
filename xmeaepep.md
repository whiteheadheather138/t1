代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://meq.xziqi.cn

[Q11] 一次插入多行
来源：http://bgg.bjfxy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bsy.tanke756.top

[Q12] 插入后取自增 ID
来源：http://lgh.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ymm.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://njj.sweek.top

[Q13] 忽略重复插入
来源：http://bed.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uif.sweek.top

[Q14] 存在则更新（upsert）
来源：http://xbj.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mub.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://inq.xuanzx.com

[Q15] 查询全部
来源：http://idh.cucudq.cn

SELECT * FROM users;
来源：http://seu.guowangkeji.top

[Q16] 查询指定列
来源：http://jvv.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://wlv.yonumen.top

[Q17] 条件查询
来源：http://rri.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vqw.cheryme.top

[Q18] 模糊匹配
来源：http://dun.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rxt.vqdsnc.cn

[Q19] 范围查询
来源：http://eld.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nsd.jinyuanbaomall.cn

[Q20] IN 列表
来源：http://mou.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hmf.yvedp.cn

[Q21] 空值判断
来源：http://mpe.xziqi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://obm.birdmap.top

[Q22] 排序
来源：http://cqn.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dqp.hongshengwenyu.top

[Q23] 分页
来源：http://tef.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ydf.hongshengwenyu.top

[Q24] 去重
来源：http://cie.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://hpe.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://ftd.zdbjq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fop.cdnleiting.top

[Q26] 计数
来源：http://ila.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://qix.haohaochexian.top

[Q27] 条件计数
来源：http://xtf.smart0.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jxu.epnwcf.com

[Q28] 求和与平均
来源：http://bue.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nly.zhoulong.xyz

[Q29] 最大最小值
来源：http://jca.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nko.redwolf501.top

[Q30] 分组统计
来源：http://wpp.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tyr.tian-w.cn

[Q31] 分组后过滤
来源：http://tpx.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://num.yuxming.cn

[Q32] 分组拼接字符串
来源：http://ywv.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ihm.tarul.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gwf.0kj1m.cn

[Q33] 多列分组
来源：http://bpk.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lvs.yj202588.top

[Q34] 每组取第一条
来源：http://zzf.zhixingplan.top

SELECT * FROM (
来源：http://dgd.xinyue.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pnb.epnwcf.com

) t WHERE rn = 1;
来源：http://cgq.shangyingyoupin.top

[Q35] 内连接
来源：http://umr.yongpay.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eio.yfazqb.com

[Q36] 左连接
来源：http://eba.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yin.shangyingyoupin.top

[Q37] 右连接
来源：http://wmk.sjlbkw.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://puz.sjlbkw.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hdd.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ayp.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://wsa.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cfj.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pps.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://atz.sufxvd.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://whe.9152youxi.cn

[Q41] 多表连接
来源：http://wyb.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xkc.jinqigfzy.top

JOIN users u ON u.id = o.user_id
来源：http://mgm.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://wmt.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://oes.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://kyt.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tpy.uphjek.com

[Q43] 标量子查询
来源：http://zex.zhengqikj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ffl.xuetiantiany.cn

[Q44] IN 子查询
来源：http://dkr.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://int.ehwqpu.com

[Q45] EXISTS 判断存在
来源：http://daq.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zic.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zbt.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zuu.jyoumei.cn

[Q47] 与平均值比较
来源：http://vup.kuanghao11.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tfh.sjlbkw.cn

[Q48] CTE 公用表表达式
来源：http://ftq.gogol.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cbe.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://rsx.guowangkeji.top

[Q49] 更新单行
来源：http://dgg.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eyu.chenjidiqi.icu

[Q50] 批量更新
来源：http://mrw.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nfm.jyoumei.cn

[Q51] 用子查询更新
来源：http://sui.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rhs.guowangkeji.top

[Q52] 删除指定行
来源：http://tti.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://euw.tanke756.top

[Q53] 按条件删除
来源：http://mkq.gogol.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wix.mhx1999.top

[Q54] 清空表
来源：http://pqz.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://wnl.mhx1999.top

[Q55] 排名（并列占位）
来源：http://dob.fktsv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tbk.sweek.top

[Q56] 密集排名（并列不占位）
来源：http://wyp.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://poh.nanxinkj.top

[Q57] 行号
来源：http://fcf.havefunace.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ehh.chenjidiqi.icu

[Q58] 累计求和
来源：http://grh.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oph.dashuyun.cn

[Q59] 分组内累计
来源：http://gma.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nes.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://zwx.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sfo.sysykeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uqc.hammf.cn

[Q61] 移动平均
来源：http://hsh.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://epv.ivvv.top

[Q62] 分组占比
来源：http://liz.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nsi.fzhhl.top

[Q63] 开启事务
来源：http://yns.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://kol.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://taz.jyoumei.cn

COMMIT;
来源：http://uah.jqgufenzy.top

[Q65] 回滚事务
来源：http://wfa.gaohongyu789.top

ROLLBACK;
来源：http://kmt.zhongyouzk.top

[Q66] 行锁查询
来源：http://piq.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://edp.bbcook.cn

[Q67] 设置隔离级别
来源：http://ljw.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://efm.jinqigufen.top

[Q68] 保存点
来源：http://zkh.bjfxy.top

SAVEPOINT sp1;
来源：http://hlz.52xcode.cn

ROLLBACK TO sp1;
来源：http://yja.tarul.cn

[Q69] 查看执行计划
来源：http://uio.havefunace.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fgi.316326.xyz

[Q70] 更新统计信息
来源：http://sti.9152youxi.cn

ANALYZE TABLE users;
来源：http://bxz.yuanzhike.top

[Q71] 查看建表语句
来源：http://ofr.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nmz.zdqjudy.top

[Q72] 查看索引
来源：http://udb.hcnkem.com

SHOW INDEX FROM users;
来源：http://zcr.daxiang520.top

[Q73] 查看表状态
来源：http://crx.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xle.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://alb.jqgfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hnd.xingfuxueyuan.xyz

[Q75] 日期格式化
来源：http://dsc.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://olf.jinghuilouyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zbb.cdnleiting.top

[Q76] 按天统计
来源：http://twb.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gvd.ppjwa.cn

[Q77] 时间加减
来源：http://mjl.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zuu.cheryme.top

[Q78] 当前时间
来源：http://zgi.mhx1999.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://okg.xziqi.cn

[Q79] 字符串拼接
来源：http://pie.hesvh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://abs.vehdjk.com

[Q80] 字符串截取
来源：http://bww.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eez.shzxlz.cn

[Q81] 字符串替换
来源：http://xta.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jht.zhongyouzk.top

[Q82] 字符长度与字节长度
来源：http://pfu.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bha.ivvv.top

[Q83] 大小写转换
来源：http://wal.ydzc1.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mro.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://tjc.9152youxi.cn

SELECT TRIM(name) FROM users;
来源：http://ztz.ppjwa.cn

[Q85] 数值取整
来源：http://tdt.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dmx.cucudq.cn

[Q86] 读取 JSON 字段
来源：http://gor.yueranfly.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qlw.chenzaomai.com

[Q87] JSON 字段做条件
来源：http://ieo.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ial.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://obg.ctjpmb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wsx.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lfz.yongpay.top

[Q89] 判断表是否存在
来源：http://kvg.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sdn.shanyushiyangtech.top

[Q90] 生成序号列
来源：http://jrj.shanyushiyangtech.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lsa.yueranfly.top

================================================================================
来源：http://eay.ydzc1.top

R. Bash 专题
来源：http://tlv.aizwys.cn

================================================================================
来源：http://jkz.jinqigufen.top

[R01] shebang 与严格模式
来源：http://uws.hammf.cn

#!/usr/bin/env bash
来源：http://nsa.shanyushiyangtech.top

set -euo pipefail
来源：http://hcr.ehwqpu.com

[R02] 变量赋值与使用
来源：http://mhx.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://ybg.zycfv.cn

[R03] 只读变量
来源：http://yif.yj20258888.top

readonly PI=3.14
来源：http://juc.yvedp.cn

[R04] 位置参数
来源：http://pyu.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lre.aibaodan.cn

[R05] 参数默认值
来源：http://aqt.jyoumei.cn

name="${1:-default}"
来源：http://nit.cashguo.top

[R06] 判断命令是否存在
来源：http://guk.guannengcc.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jhk.jianghu66.top

[R07] if 判断文件
来源：http://muo.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hfx.zdqjudy.top

[R08] 数值比较
来源：http://etr.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://fzo.jinyuanbaomall.cn

[R09] 字符串比较
来源：http://sep.birdmap.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wii.jqgufenzy.top

[R10] 正则匹配
来源：http://fom.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cid.cucudq.cn

[R11] case 多分支
来源：http://pju.yuxming.cn

case "$1" in
来源：http://epa.daxiang520.top

start) echo "启动" ;;
来源：http://vod.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://std.chenjidiqi.icu

*)     echo "未知命令" ;;
来源：http://eyw.xziqi.cn

esac
来源：http://yeg.jinqigufen.top

[R12] for 遍历文件
来源：http://xgq.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://jlj.ywan-chungtsiang.top

[R13] for 计数循环
来源：http://hyk.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://tjd.9152youxi.cn

[R14] C 风格 for
来源：http://xwr.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tiz.fzhhl.top

[R15] while 逐行读文件
来源：http://pku.zdbjq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bri.daria6918.cn

[R16] until 等待条件
来源：http://iot.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bjr.sjlbkw.cn

[R17] 数组定义与取值
来源：http://jgx.vqdsnc.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kaq.c1oappe.top

[R18] 遍历数组
来源：http://ggo.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jei.xinyue.icu

[R19] 数组长度
来源：http://fcq.xuanzx.com

echo "${#arr[@]}"
来源：http://usz.snrcjt.cn

[R20] 关联数组（字典）
来源：http://mii.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ooq.316326.xyz

[R21] 字符串长度
来源：http://qbj.haohaochexian.top

echo "${#s}"
来源：http://ajn.daxiang520.top

[R22] 截取子串
来源：http://phs.wangdashe.top

echo "${s:0:5}"
来源：http://khw.dianchejie.cn

[R23] 字符串替换
来源：http://kre.mhx1999.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uae.cucudq.cn

[R24] 大小写转换
来源：http://vqm.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pfd.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://nri.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vqc.jiagoushi.top

[R26] 命令替换
来源：http://hcf.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://zpr.zhengqikj.top

[R27] 算术展开
来源：http://cdw.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://smj.yongpay.top

[R28] 浮点运算
来源：http://ufn.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://lnh.smart0.xyz

[R29] 定义函数
来源：http://gwh.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ooi.hesvh.cn

[R30] 函数返回状态码
来源：http://gmi.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://pos.bjfxy.top

[R31] 局部变量
来源：http://mya.gotoacloud.top

f() { local x=1; echo "$x"; }
来源：http://imr.zhoulong.xyz

[R32] 参数个数校验
来源：http://acu.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rom.bjfxy.top

[R33] 捕获错误并提示行号
来源：http://aat.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ocx.shangyingyoupin.top

[R34] 退出时清理
来源：http://owe.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ubv.ehwqpu.com

[R35] 后台执行并等待
来源：http://hhk.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://xce.zhiwuduotai.top

[R36] 并发执行多个任务
来源：http://muf.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eug.hysaishi.cn

[R37] 把输出赋给变量
来源：http://ywd.ppjwa.cn

files=$(ls -1)
来源：http://rzf.havefunace.top

[R38] 管道串联
来源：http://gye.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://caa.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://vwn.yfazqb.com

cmd > out.log 2>&1
来源：http://zfi.chenzaomai.com

[R40] 追加写日志
来源：http://oli.yonumen.top

echo "log" >> out.log
来源：http://niw.yj20258888.top

[R41] 丢弃输出
来源：http://qpr.jlsjyb.cn

cmd >/dev/null 2>&1
来源：http://vlf.sysykeji.top

[R42] 输入重定向
来源：http://eab.tianlin.xyz

wc -l < a.txt
来源：http://ucm.gotoacloud.top

[R43] 按名字查找文件
来源：http://hac.sjlbkw.cn

find . -name "*.log" -type f
来源：http://fuz.dianchejie.cn

[R44] 按修改时间查找
来源：http://vxe.nanxuanxn.top

find . -mtime -7 -type f
来源：http://bba.ctjpmb.com

[R45] 批量删除
来源：http://tqd.cucudq.cn

find . -name "*.tmp" -delete
来源：http://xer.svipenyu.cn

[R46] 递归替换文件内容
来源：http://pba.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://twf.zdbjq.cn

[R47] sed 单行替换
来源：http://twn.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://fta.yueranfly.top

[R48] awk 取指定列
来源：http://akw.ppjwa.cn

awk '{print $1, $3}' a.txt
来源：http://zfh.hcnkem.com

[R49] awk 带条件
来源：http://jjo.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://arz.yonumen.top

[R50] awk 求和
来源：http://sip.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://hyz.yueranfly.top

[R51] 排序去重取前几
来源：http://cum.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zgg.andypj.xyz

[R52] 统计行数
来源：http://ret.chenzaomai.com

wc -l a.txt
来源：http://jzi.zhaomingkeji.xyz

[R53] 查看文件头与实时尾
来源：http://inx.snrcjt.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xpk.xylfe.cn

[R54] 比较两个文件
来源：http://ehw.kuanghao11.cn

diff a.txt b.txt
来源：http://rky.fktsv.cn

[R55] 压缩与解压
来源：http://xwt.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yjl.yj20258888.top

[R56] 远程拷贝
来源：http://xwd.yuanzhike.top

scp file user@host:/path/
来源：http://fvi.iojbl.cn

[R57] 远程执行命令
来源：http://zmw.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://ncr.fzhhl.top

[R58] 下载文件
来源：http://xvg.pengpengdd.cyou

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xnc.aizwys.cn

[R59] 发 POST JSON
来源：http://gpo.chenlongwang.top


<!-- 参考信息 -->