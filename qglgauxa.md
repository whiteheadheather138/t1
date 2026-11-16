代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://wxo.pycfn.com

[Q07] 删除表
来源：http://xzd.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://igb.sxryk.cn

[Q08] 创建普通索引
来源：http://ghk.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://skk.fengsongda.top

[Q09] 创建唯一索引
来源：http://ckk.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bhs.snrcjt.cn

[Q10] 插入单行
来源：http://zdm.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mte.epnwcf.com

[Q11] 一次插入多行
来源：http://zno.aizwys.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xlh.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://tbq.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kzk.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xlq.ppjwa.cn

[Q13] 忽略重复插入
来源：http://nte.yj20258.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vae.shzxlz.cn

[Q14] 存在则更新（upsert）
来源：http://iph.daria6918.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ugd.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uzz.zhoulong.xyz

[Q15] 查询全部
来源：http://xea.andypj.xyz

SELECT * FROM users;
来源：http://vyv.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://lyb.yuanzhike.top

SELECT id, name FROM users;
来源：http://lfn.zhijiandao.cn

[Q17] 条件查询
来源：http://vjx.zdqjudy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dol.zycfv.cn

[Q18] 模糊匹配
来源：http://tsn.gogol.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qri.52xcode.cn

[Q19] 范围查询
来源：http://ucl.dianchejie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kfe.316326.xyz

[Q20] IN 列表
来源：http://xgl.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pkv.xinyue.icu

[Q21] 空值判断
来源：http://qyc.birdmap.top

SELECT * FROM users WHERE email IS NULL;
来源：http://phy.tanke756.top

[Q22] 排序
来源：http://azk.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://otc.hammf.cn

[Q23] 分页
来源：http://vzo.hongshengwenyu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tji.9152youxi.cn

[Q24] 去重
来源：http://irs.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://trp.bjfxy.top

[Q25] 只取前 N 条
来源：http://vda.jinghuilouyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://osm.zhoulong.xyz

[Q26] 计数
来源：http://sdg.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://jzw.meibo888.top

[Q27] 条件计数
来源：http://rth.haohaochexian.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vnq.sweek.top

[Q28] 求和与平均
来源：http://txi.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://but.sweek.top

[Q29] 最大最小值
来源：http://zcx.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://giq.vehdjk.com

[Q30] 分组统计
来源：http://gwn.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vzr.jinqigufen.top

[Q31] 分组后过滤
来源：http://ngh.aizwys.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hyd.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://xoh.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://afk.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vbv.svipenyu.cn

[Q33] 多列分组
来源：http://zos.jyoumei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ahv.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://tcj.yfazqb.com

SELECT * FROM (
来源：http://ter.zhoulong.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nle.hnxiangtu.top

) t WHERE rn = 1;
来源：http://jfk.fktsv.cn

[Q35] 内连接
来源：http://fua.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ghf.redwolf501.top

[Q36] 左连接
来源：http://ywf.guannengcc.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rdm.ywan-chungtsiang.top

[Q37] 右连接
来源：http://yvh.guowangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gcu.c1oappe.top

[Q38] 全外连接（PostgreSQL）
来源：http://hbt.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lkk.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://umh.xinyue.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://rno.shanyushiyangtech.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://twe.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hwg.guannengcc.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aqq.ivvv.top

[Q41] 多表连接
来源：http://yos.yj20258888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xqh.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://xpl.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://mnz.daxiang520.top

[Q42] 连接条件附加过滤
来源：http://nxs.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://dfi.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://laa.feifeiyinyue.top

[Q43] 标量子查询
来源：http://dvl.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jnp.shzxlz.cn

[Q44] IN 子查询
来源：http://mui.wangdashe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wky.316326.xyz

[Q45] EXISTS 判断存在
来源：http://xxo.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://izx.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jeb.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://abl.gaohongyu789.top

[Q47] 与平均值比较
来源：http://apu.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rbz.jinyuanbaomall.cn

[Q48] CTE 公用表表达式
来源：http://iey.uphjek.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lpl.gogol.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://fcx.wangshuangyany.cn

[Q49] 更新单行
来源：http://oby.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cao.tanke756.top

[Q50] 批量更新
来源：http://mdv.quarkkingdee.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dit.pycfn.com

[Q51] 用子查询更新
来源：http://iox.tian-w.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fzm.zhixingplan.top

[Q52] 删除指定行
来源：http://fqu.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://cyk.bbcook.cn

[Q53] 按条件删除
来源：http://thr.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tmk.dianchejie.cn

[Q54] 清空表
来源：http://izb.sjlbkw.cn

TRUNCATE TABLE logs;
来源：http://tin.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://iet.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dft.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://dgb.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ucg.andypj.xyz

[Q57] 行号
来源：http://oqh.jinyuanbaomall.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pue.nwbrower.top

[Q58] 累计求和
来源：http://cmp.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fwe.fktsv.cn

[Q59] 分组内累计
来源：http://efe.yvedp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://crz.jinghuilouyu.cn

[Q60] 取上一行 / 下一行
来源：http://ysu.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://akw.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vob.tanke756.top

[Q61] 移动平均
来源：http://yrt.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://byo.xylfe.cn

[Q62] 分组占比
来源：http://tkp.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lbe.sxryk.cn

[Q63] 开启事务
来源：http://wjp.hysaishi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jkh.tarul.cn

[Q64] 提交事务
来源：http://lek.ctjpmb.com

COMMIT;
来源：http://jix.meibo888.top

[Q65] 回滚事务
来源：http://zsx.cheryme.top

ROLLBACK;
来源：http://lne.pycfn.com

[Q66] 行锁查询
来源：http://cdr.fzhhl.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bpl.bjfxy.top

[Q67] 设置隔离级别
来源：http://dze.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rsu.nwbrower.top

[Q68] 保存点
来源：http://nuf.jlsjyb.cn

SAVEPOINT sp1;
来源：http://yer.zhixingplan.top

ROLLBACK TO sp1;
来源：http://hvm.shanyushiyangtech.top

[Q69] 查看执行计划
来源：http://qsp.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vwz.nwbrower.top

[Q70] 更新统计信息
来源：http://laq.jianghu66.top

ANALYZE TABLE users;
来源：http://uvs.uphjek.com

[Q71] 查看建表语句
来源：http://ynd.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zsg.jqgfzy.top

[Q72] 查看索引
来源：http://coh.uphjek.com

SHOW INDEX FROM users;
来源：http://lxt.iojbl.cn

[Q73] 查看表状态
来源：http://omz.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://enp.ivvv.top

[Q74] 强制使用索引
来源：http://psn.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ofs.fehbvm.com

[Q75] 日期格式化
来源：http://wee.gzhubu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xtf.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sww.fktsv.cn

[Q76] 按天统计
来源：http://aot.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jnh.snrcjt.cn

[Q77] 时间加减
来源：http://dus.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zee.chenlongwang.top

[Q78] 当前时间
来源：http://oxq.birdmap.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dhd.andypj.xyz

[Q79] 字符串拼接
来源：http://pkm.dashuyun.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://koz.nwbrower.top

[Q80] 字符串截取
来源：http://veg.chenlongwang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wvl.yongpay.top

[Q81] 字符串替换
来源：http://czs.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jhw.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://kzt.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://foq.jiagoushi.top

[Q83] 大小写转换
来源：http://xfq.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vqr.svipenyu.cn

[Q84] 去除首尾空格
来源：http://org.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://zqy.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://smq.quarkkingdee.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hqe.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://wsr.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tan.wangdashe.top

[Q87] JSON 字段做条件
来源：http://dew.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ejs.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://sad.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pyq.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oje.hysaishi.cn

[Q89] 判断表是否存在
来源：http://dbt.xingfuxueyuan.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://btz.yj20258888.top

[Q90] 生成序号列
来源：http://pgr.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xyb.zhongyouzk.top

================================================================================
来源：http://ggr.tanke756.top

R. Bash 专题
来源：http://typ.yvedp.cn

================================================================================
来源：http://ezg.ydjk.org.cn

[R01] shebang 与严格模式
来源：http://jan.sxryk.cn

#!/usr/bin/env bash
来源：http://tch.hammf.cn

set -euo pipefail
来源：http://qfx.316326.xyz

[R02] 变量赋值与使用
来源：http://jxs.yvedp.cn

name="Tom"; echo "$name"
来源：http://uej.c1oappe.top

[R03] 只读变量
来源：http://tcw.shanyushiyangkeji.top

readonly PI=3.14
来源：http://ldf.aibaodan.cn

[R04] 位置参数
来源：http://cbb.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mls.tian-w.cn

[R05] 参数默认值
来源：http://kct.meibo888.top

name="${1:-default}"
来源：http://zkv.fengsongda.top

[R06] 判断命令是否存在
来源：http://zwn.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zwz.epnwcf.com

[R07] if 判断文件
来源：http://qqt.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eez.ehwqpu.com

[R08] 数值比较
来源：http://fii.zhoulong.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://pgu.jyoumei.cn

[R09] 字符串比较
来源：http://dzq.c1oappe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qub.wangshuangyany.cn

[R10] 正则匹配
来源：http://cwb.sjlbkw.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://haj.ydzc1.top

[R11] case 多分支
来源：http://yeq.jiagoushi.top

case "$1" in
来源：http://jbh.zhongyouzk.top

start) echo "启动" ;;
来源：http://iar.iojbl.cn

stop)  echo "停止" ;;
来源：http://wnq.jinghuilouyu.cn

*)     echo "未知命令" ;;
来源：http://jvf.hesvh.cn

esac
来源：http://dwn.cucudq.cn

[R12] for 遍历文件
来源：http://nkt.hywenlv.cn

for f in *.txt; do echo "$f"; done
来源：http://bsw.dianchejie.cn

[R13] for 计数循环
来源：http://dge.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://cxq.zdbjq.cn

[R14] C 风格 for
来源：http://cya.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jhr.zdqjudy.top

[R15] while 逐行读文件
来源：http://mly.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lsw.jiagoushi.top

[R16] until 等待条件
来源：http://ghs.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://piz.quarkkingdee.top

[R17] 数组定义与取值
来源：http://wlr.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://gxr.ppjwa.cn

[R18] 遍历数组
来源：http://kdi.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lbe.52xcode.cn

[R19] 数组长度
来源：http://ybj.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://zyx.havefunace.top

[R20] 关联数组（字典）
来源：http://lex.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aam.pycfn.com

[R21] 字符串长度
来源：http://lth.ywan-chungtsiang.top

echo "${#s}"
来源：http://vzm.shanyushiyangkeji.top

[R22] 截取子串
来源：http://fff.daria6918.cn

echo "${s:0:5}"
来源：http://vdz.yj20258.top

[R23] 字符串替换
来源：http://pfd.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jfc.feifeiyinyue.top

[R24] 大小写转换
来源：http://aun.jinqigfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://cjd.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://boz.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tts.jianghu66.top

[R26] 命令替换
来源：http://cdx.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://xci.zhongyouzk.top

[R27] 算术展开
来源：http://wkd.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://pzs.hnxiangtu.top

[R28] 浮点运算
来源：http://zmm.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://uzv.0kj1m.cn

[R29] 定义函数
来源：http://hwb.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nlb.zhengqikj.top

[R30] 函数返回状态码
来源：http://feo.zhoulong.xyz

f() { return 0; }; f || echo "失败了"
来源：http://pfo.jinghuilouyu.cn

[R31] 局部变量
来源：http://tyi.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://prs.ppjwa.cn

[R32] 参数个数校验
来源：http://vzi.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zfr.cheryme.top

[R33] 捕获错误并提示行号
来源：http://mop.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://unq.wangshuangyany.cn

[R34] 退出时清理
来源：http://aqi.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://uut.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://bxe.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://izg.svipenyu.cn

[R36] 并发执行多个任务
来源：http://mzf.jinghuilouyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hdh.cashguo.top

[R37] 把输出赋给变量
来源：http://iez.fengsongda.top

files=$(ls -1)
来源：http://kej.sxryk.cn

[R38] 管道串联
来源：http://cmt.dianchejie.cn

cat a.txt | grep -i error | wc -l
来源：http://kzk.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://pby.kuanghao11.cn

cmd > out.log 2>&1
来源：http://heh.xylfe.cn

[R40] 追加写日志
来源：http://nic.hongshengwenyu.top

echo "log" >> out.log
来源：http://whw.yfazqb.com

[R41] 丢弃输出
来源：http://jws.yuxming.cn

cmd >/dev/null 2>&1
来源：http://hpl.zhoulong.xyz

[R42] 输入重定向
来源：http://gav.jinqigufen.top

wc -l < a.txt
来源：http://lps.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://gto.cqqwz.cn

find . -name "*.log" -type f
来源：http://rhn.gaohongyu789.top

[R44] 按修改时间查找
来源：http://fzk.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://trq.yuxming.cn

[R45] 批量删除
来源：http://mvr.yfazqb.com

find . -name "*.tmp" -delete
来源：http://jdv.sweek.top

[R46] 递归替换文件内容
来源：http://xvh.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wzf.52xcode.cn

[R47] sed 单行替换
来源：http://sah.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://kkk.aizwys.cn

[R48] awk 取指定列
来源：http://cxi.shanyushiyangkeji.top

awk '{print $1, $3}' a.txt
来源：http://cdh.fanxiaobao.xyz

[R49] awk 带条件
来源：http://bsd.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jrn.iojbl.cn

[R50] awk 求和
来源：http://xwz.vehdjk.com

awk '{s += $2} END {print s}' a.txt
来源：http://hno.tianlin.xyz

[R51] 排序去重取前几
来源：http://hpd.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hxs.jinqigfzy.top

[R52] 统计行数
来源：http://dkx.jiagoushi.top

wc -l a.txt
来源：http://fcr.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://tuy.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xhr.zhongyouzk.top

[R54] 比较两个文件
来源：http://fqy.jqgfzy.top

diff a.txt b.txt
来源：http://kzu.zhengqikj.top

[R55] 压缩与解压
来源：http://veh.yangfankeji.com


<!-- 参考信息 -->