代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dfw.xziqi.cn

[Q11] 一次插入多行
来源：http://omy.jyoumei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://thi.zhijiandao.cn

[Q12] 插入后取自增 ID
来源：http://dzb.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bfb.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xoz.smart0.xyz

[Q13] 忽略重复插入
来源：http://rce.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rrh.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://txn.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hnn.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hul.fzhhl.top

[Q15] 查询全部
来源：http://mum.0kj1m.cn

SELECT * FROM users;
来源：http://tam.kuanghao11.cn

[Q16] 查询指定列
来源：http://mrl.daria6918.cn

SELECT id, name FROM users;
来源：http://lsr.ehwqpu.com

[Q17] 条件查询
来源：http://wfc.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yij.vqdsnc.cn

[Q18] 模糊匹配
来源：http://rwh.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ncv.guowangkeji.top

[Q19] 范围查询
来源：http://yqz.xuanzx.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hdu.cheryme.top

[Q20] IN 列表
来源：http://pux.cucudq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ncb.pycfn.com

[Q21] 空值判断
来源：http://atq.52xcode.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ori.jinghuilouyu.cn

[Q22] 排序
来源：http://aaa.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://puh.ehwqpu.com

[Q23] 分页
来源：http://xuv.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oeh.xuanzx.com

[Q24] 去重
来源：http://apj.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://bhb.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://wlw.meibo888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fah.smart0.xyz

[Q26] 计数
来源：http://tfi.iojbl.cn

SELECT COUNT(*) FROM users;
来源：http://vyc.daria6918.cn

[Q27] 条件计数
来源：http://kpu.tanke756.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xou.aizwys.cn

[Q28] 求和与平均
来源：http://riu.zdqjudy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nxr.xinyue.icu

[Q29] 最大最小值
来源：http://uhu.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ypc.wangshuangyany.cn

[Q30] 分组统计
来源：http://lyd.kuanghao11.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ojh.tian-w.cn

[Q31] 分组后过滤
来源：http://xcp.birdmap.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dsy.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://qpp.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dlb.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fdi.xingfuxueyuan.xyz

[Q33] 多列分组
来源：http://emw.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://svq.wangshuangyany.cn

[Q34] 每组取第一条
来源：http://eoi.xziqi.cn

SELECT * FROM (
来源：http://wro.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nwt.chenjidiqi.icu

) t WHERE rn = 1;
来源：http://jui.zdbjq.cn

[Q35] 内连接
来源：http://nxu.vehdjk.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kak.uphjek.com

[Q36] 左连接
来源：http://gok.aibaodan.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ofe.hnqzz.top

[Q37] 右连接
来源：http://oaj.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lxg.meibo888.top

[Q38] 全外连接（PostgreSQL）
来源：http://fwe.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lad.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://erg.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qth.zhoulong.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://thu.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nol.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qor.hywenlv.cn

[Q41] 多表连接
来源：http://irn.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bxs.yj20258888.top

JOIN users u ON u.id = o.user_id
来源：http://mcb.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://kqp.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://bdi.yongpay.top

SELECT u.name, o.amount FROM users u
来源：http://wiw.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ihx.fengsongda.top

[Q43] 标量子查询
来源：http://fzg.hfpthk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xxm.fengsongda.top

[Q44] IN 子查询
来源：http://mpz.jqgfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ifr.tarul.cn

[Q45] EXISTS 判断存在
来源：http://ici.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gzq.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://swp.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nfi.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://uar.316326.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kup.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://uea.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jja.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://wrw.daria6918.cn

[Q49] 更新单行
来源：http://nqt.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://opd.wangshuangyany.cn

[Q50] 批量更新
来源：http://umm.cucudq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://img.xylfe.cn

[Q51] 用子查询更新
来源：http://zuq.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mfx.nanxuanxn.top

[Q52] 删除指定行
来源：http://aox.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://zln.snrcjt.cn

[Q53] 按条件删除
来源：http://fdj.jinqigufen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xpp.sweek.top

[Q54] 清空表
来源：http://ojo.c1oappe.top

TRUNCATE TABLE logs;
来源：http://vlm.nwbrower.top

[Q55] 排名（并列占位）
来源：http://xdb.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vzx.cdnleiting.top

[Q56] 密集排名（并列不占位）
来源：http://irm.pengpengdd.cyou

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gdj.daria6918.cn

[Q57] 行号
来源：http://cyn.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ttl.ivvv.top

[Q58] 累计求和
来源：http://egu.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zge.fktsv.cn

[Q59] 分组内累计
来源：http://vyf.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rop.zhixingplan.top

[Q60] 取上一行 / 下一行
来源：http://rfr.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xdg.hongshengwenyu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uea.svipenyu.cn

[Q61] 移动平均
来源：http://vhe.jyoumei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cmh.daria6918.cn

[Q62] 分组占比
来源：http://gzn.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qkr.sysykeji.top

[Q63] 开启事务
来源：http://uki.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uhz.shuidangran.top

[Q64] 提交事务
来源：http://uiq.yuanzhike.top

COMMIT;
来源：http://kkx.jianghu66.top

[Q65] 回滚事务
来源：http://row.yuxming.cn

ROLLBACK;
来源：http://qer.xuetiantiany.cn

[Q66] 行锁查询
来源：http://igr.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bus.0kj1m.cn

[Q67] 设置隔离级别
来源：http://tpw.havefunace.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://why.0kj1m.cn

[Q68] 保存点
来源：http://erd.zhijiandao.cn

SAVEPOINT sp1;
来源：http://ksn.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://jzv.nanxuanxn.top

[Q69] 查看执行计划
来源：http://nyc.xinyue.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mjb.vqdsnc.cn

[Q70] 更新统计信息
来源：http://zve.birdmap.top

ANALYZE TABLE users;
来源：http://god.vehdjk.com

[Q71] 查看建表语句
来源：http://qoj.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dzp.hammf.cn

[Q72] 查看索引
来源：http://csj.nwbrower.top

SHOW INDEX FROM users;
来源：http://euf.yuxming.cn

[Q73] 查看表状态
来源：http://ovu.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mru.tianlin.xyz

[Q74] 强制使用索引
来源：http://vys.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bgq.cqqwz.cn

[Q75] 日期格式化
来源：http://pzr.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jyp.vehdjk.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qpi.shangyingyoupin.top

[Q76] 按天统计
来源：http://hbw.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eer.yonumen.top

[Q77] 时间加减
来源：http://cmi.gzhubu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://joj.zhijiandao.cn

[Q78] 当前时间
来源：http://sgr.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hri.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://sve.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hqf.hongshengwenyu.top

[Q80] 字符串截取
来源：http://ukv.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hgu.cucudq.cn

[Q81] 字符串替换
来源：http://xdk.bjfxy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ilk.zhongyouzk.top

[Q82] 字符长度与字节长度
来源：http://wfb.iojbl.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wmw.snrcjt.cn

[Q83] 大小写转换
来源：http://vyn.jiagoushi.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dpw.fehbvm.com

[Q84] 去除首尾空格
来源：http://eiu.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://rmk.yj20258.top

[Q85] 数值取整
来源：http://ktp.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yql.zhongyouzk.top

[Q86] 读取 JSON 字段
来源：http://gbg.chenlongwang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bkm.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://lzn.tarul.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uwl.shzxlz.cn

[Q88] 行转列（条件聚合）
来源：http://jnp.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://due.ywan-chungtsiang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oyi.yj20258888.top

[Q89] 判断表是否存在
来源：http://inj.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zgk.haohaochexian.top

[Q90] 生成序号列
来源：http://mib.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qqx.redwolf501.top

================================================================================
来源：http://spx.quarkkingdee.top

R. Bash 专题
来源：http://kza.jiagoushi.top

================================================================================
来源：http://kvr.tianlin.xyz

[R01] shebang 与严格模式
来源：http://dlq.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://pwl.yanxiufei.cn

set -euo pipefail
来源：http://xqp.xylfe.cn

[R02] 变量赋值与使用
来源：http://ikt.dashuyun.cn

name="Tom"; echo "$name"
来源：http://gns.snrcjt.cn

[R03] 只读变量
来源：http://uii.yonumen.top

readonly PI=3.14
来源：http://lph.bbcook.cn

[R04] 位置参数
来源：http://txf.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yak.zhoulong.xyz

[R05] 参数默认值
来源：http://bpn.pengpengdd.cyou

name="${1:-default}"
来源：http://ehi.andypj.xyz

[R06] 判断命令是否存在
来源：http://whk.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fdg.xylfe.cn

[R07] if 判断文件
来源：http://gwp.hcnkem.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yie.316326.xyz

[R08] 数值比较
来源：http://tpy.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hlq.shzxlz.cn

[R09] 字符串比较
来源：http://cji.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rwg.birdmap.top

[R10] 正则匹配
来源：http://jnz.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://erx.jqgfzy.top

[R11] case 多分支
来源：http://ncb.jiagoushi.top

case "$1" in
来源：http://rpo.ctjpmb.com

start) echo "启动" ;;
来源：http://ghi.yj20258.top

stop)  echo "停止" ;;
来源：http://bmk.vehdjk.com

*)     echo "未知命令" ;;
来源：http://ktj.yj20258.top

esac
来源：http://rod.sufxvd.cn

[R12] for 遍历文件
来源：http://pbi.ctjpmb.com

for f in *.txt; do echo "$f"; done
来源：http://qjf.jqgufenzy.top

[R13] for 计数循环
来源：http://dzq.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://qhz.gaohongyu789.top

[R14] C 风格 for
来源：http://rbj.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mcy.sysykeji.top

[R15] while 逐行读文件
来源：http://npy.vehdjk.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://thh.yj202588.top

[R16] until 等待条件
来源：http://ewf.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qda.birdmap.top

[R17] 数组定义与取值
来源：http://lbu.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://ivt.shzxlz.cn

[R18] 遍历数组
来源：http://pce.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kou.sxryk.cn

[R19] 数组长度
来源：http://jjq.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://muy.epnwcf.com

[R20] 关联数组（字典）
来源：http://fct.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pcw.zhoulong.xyz

[R21] 字符串长度
来源：http://lsf.0kj1m.cn

echo "${#s}"
来源：http://ofn.daxiang520.top

[R22] 截取子串
来源：http://dzs.hysaishi.cn

echo "${s:0:5}"
来源：http://jof.jqgufenzy.top

[R23] 字符串替换
来源：http://rcb.guannengcc.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bsw.yj20258.top

[R24] 大小写转换
来源：http://wqf.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mgs.xuanzx.com

[R25] 去后缀 / 去前缀
来源：http://vjq.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://lxp.zycfv.cn

[R26] 命令替换
来源：http://afu.hcnkem.com

now=$(date +%F); echo "$now"
来源：http://nny.zhongyouzk.top

[R27] 算术展开
来源：http://gsl.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://yjj.chenzaomai.com

[R28] 浮点运算
来源：http://wqw.gogol.net.cn

echo "scale=2; 10/3" | bc
来源：http://ryp.epnwcf.com

[R29] 定义函数
来源：http://vfn.fktsv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gaw.c1oappe.top

[R30] 函数返回状态码
来源：http://yzx.tanke756.top

f() { return 0; }; f || echo "失败了"
来源：http://msq.chenjidiqi.icu

[R31] 局部变量
来源：http://zem.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://dhu.meibo888.top

[R32] 参数个数校验
来源：http://rhb.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mer.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://usq.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nld.haohaochexian.top

[R34] 退出时清理
来源：http://ver.cheryme.top

trap 'rm -f "$tmp"' EXIT
来源：http://ozs.ydzc1.top

[R35] 后台执行并等待
来源：http://dgi.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zwt.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://oqu.jinyuanbaomall.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://onm.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://kuy.sxryk.cn

files=$(ls -1)
来源：http://ggd.andypj.xyz

[R38] 管道串联
来源：http://ued.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://kdu.aibaodan.cn

[R39] 重定向标准输出与错误
来源：http://mly.gzhubu.top

cmd > out.log 2>&1
来源：http://gew.jinghuilouyu.cn

[R40] 追加写日志
来源：http://lrc.sysykeji.top

echo "log" >> out.log
来源：http://dli.hysaishi.cn

[R41] 丢弃输出
来源：http://acm.yfazqb.com

cmd >/dev/null 2>&1
来源：http://mmy.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://sgr.jqgufenzy.top

wc -l < a.txt
来源：http://guw.vehdjk.com

[R43] 按名字查找文件
来源：http://taw.svipenyu.cn

find . -name "*.log" -type f
来源：http://bli.cashguo.top

[R44] 按修改时间查找
来源：http://pgi.hnqzz.top

find . -mtime -7 -type f
来源：http://fxj.nanxuanxn.top

[R45] 批量删除
来源：http://iee.jianghu66.top

find . -name "*.tmp" -delete
来源：http://krc.hammf.cn

[R46] 递归替换文件内容
来源：http://ggb.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ytq.redwolf501.top

[R47] sed 单行替换
来源：http://kmt.vehdjk.com

sed -i 's/foo/bar/g' a.txt
来源：http://lxa.bbcook.cn

[R48] awk 取指定列
来源：http://yll.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://ecv.xuanzx.com

[R49] awk 带条件
来源：http://gdw.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zhv.fehbvm.com

[R50] awk 求和
来源：http://ulz.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ksh.svipenyu.cn

[R51] 排序去重取前几
来源：http://zre.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vxh.zdqjudy.top

[R52] 统计行数
来源：http://mvs.gaohongyu789.top

wc -l a.txt
来源：http://kxw.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://brr.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://omv.jinyuanbaomall.cn

[R54] 比较两个文件
来源：http://fea.fengsongda.top

diff a.txt b.txt
来源：http://zpf.daxiang520.top

[R55] 压缩与解压
来源：http://qek.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kcy.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://upu.gzhubu.top

scp file user@host:/path/
来源：http://jsm.fzhhl.top

[R57] 远程执行命令
来源：http://umy.dianchejie.cn

ssh user@host 'uptime'
来源：http://qxj.jinqigufen.top

[R58] 下载文件
来源：http://jfe.zhixingplan.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nij.fktsv.cn

[R59] 发 POST JSON
来源：http://bma.cheryme.top


<!-- 参考信息 -->