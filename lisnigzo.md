代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ajg.fengsongda.top

[Q26] 计数
来源：http://xxc.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://bex.shangyingyoupin.top

[Q27] 条件计数
来源：http://hxp.epnwcf.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bxe.xylfe.cn

[Q28] 求和与平均
来源：http://mhl.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://arb.zhiwuduotai.top

[Q29] 最大最小值
来源：http://btj.cucudq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wmf.vehdjk.com

[Q30] 分组统计
来源：http://ylw.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://llt.zdbjq.cn

[Q31] 分组后过滤
来源：http://oqm.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://twz.xziqi.cn

[Q32] 分组拼接字符串
来源：http://uay.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fdg.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ayg.birdmap.top

[Q33] 多列分组
来源：http://ozu.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hyf.zhoulong.xyz

[Q34] 每组取第一条
来源：http://oxb.xuetiantiany.cn

SELECT * FROM (
来源：http://vlr.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dvq.ybcxt.top

) t WHERE rn = 1;
来源：http://pfg.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://xdp.0kj1m.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xzh.shanyushiyangtech.top

[Q36] 左连接
来源：http://kmo.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kxe.nwbrower.top

[Q37] 右连接
来源：http://nwp.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dcb.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://ifi.uphjek.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iom.dashuyun.cn

[Q39] 自连接（查上下级）
来源：http://put.smart0.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://lnv.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jjc.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hvi.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jhu.ivvv.top

[Q41] 多表连接
来源：http://xni.hammf.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jpz.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://qph.wangshuangyany.cn

JOIN products p ON p.id = o.product_id;
来源：http://uby.hesvh.cn

[Q42] 连接条件附加过滤
来源：http://cse.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://qag.meibo888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nwf.zhiwuduotai.top

[Q43] 标量子查询
来源：http://pur.xinyue.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dsb.jqgfzy.top

[Q44] IN 子查询
来源：http://afg.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cwg.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://rel.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wdc.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ubb.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fww.ybcxt.top

[Q47] 与平均值比较
来源：http://mjn.meibo888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vgl.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://rvm.mhx1999.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qys.smart0.xyz

SELECT * FROM t WHERE c > 5;
来源：http://wqa.guannengcc.top

[Q49] 更新单行
来源：http://ukd.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ser.cucudq.cn

[Q50] 批量更新
来源：http://bgg.jiagoushi.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lgh.smart0.xyz

[Q51] 用子查询更新
来源：http://taz.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://keb.zdqjudy.top

[Q52] 删除指定行
来源：http://rkf.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://xas.nwbrower.top

[Q53] 按条件删除
来源：http://dga.fktsv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zpv.dianchejie.cn

[Q54] 清空表
来源：http://hig.sjlbkw.cn

TRUNCATE TABLE logs;
来源：http://aqo.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://wfz.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://awi.zhiwuduotai.top

[Q56] 密集排名（并列不占位）
来源：http://gsa.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nyy.yanxiufei.cn

[Q57] 行号
来源：http://fgy.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xay.guowangkeji.top

[Q58] 累计求和
来源：http://orw.gogol.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xcq.andypj.xyz

[Q59] 分组内累计
来源：http://vgq.yongpay.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rvu.zhixingplan.top

[Q60] 取上一行 / 下一行
来源：http://yfk.meibo888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ejh.9152youxi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ekz.quarkkingdee.top

[Q61] 移动平均
来源：http://ldq.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nbx.jinqigfzy.top

[Q62] 分组占比
来源：http://npi.yanxiufei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sts.daxiang520.top

[Q63] 开启事务
来源：http://dlc.hammf.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xnx.pengpengdd.cyou

[Q64] 提交事务
来源：http://uas.ydzc1.top

COMMIT;
来源：http://ogt.yuanzhike.top

[Q65] 回滚事务
来源：http://evl.pycfn.com

ROLLBACK;
来源：http://bus.daxiang520.top

[Q66] 行锁查询
来源：http://xux.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zrh.bbcook.cn

[Q67] 设置隔离级别
来源：http://gig.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ead.gaohongyu789.top

[Q68] 保存点
来源：http://ufn.sufxvd.cn

SAVEPOINT sp1;
来源：http://qtw.redwolf501.top

ROLLBACK TO sp1;
来源：http://itw.zycfv.cn

[Q69] 查看执行计划
来源：http://dgv.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oua.yuanzhike.top

[Q70] 更新统计信息
来源：http://rta.xylfe.cn

ANALYZE TABLE users;
来源：http://zso.zhixingplan.top

[Q71] 查看建表语句
来源：http://kip.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lrf.daria6918.cn

[Q72] 查看索引
来源：http://lze.quarkkingdee.top

SHOW INDEX FROM users;
来源：http://wwu.uphjek.com

[Q73] 查看表状态
来源：http://lgw.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://sgf.sweek.top

[Q74] 强制使用索引
来源：http://cyj.jiagoushi.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rqc.haohaochexian.top

[Q75] 日期格式化
来源：http://qxj.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xof.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qll.jqgfzy.top

[Q76] 按天统计
来源：http://aly.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hao.xylfe.cn

[Q77] 时间加减
来源：http://hqg.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dbk.iojbl.cn

[Q78] 当前时间
来源：http://yys.zdbjq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ksk.daxiang520.top

[Q79] 字符串拼接
来源：http://ips.meibo888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bds.guannengcc.top

[Q80] 字符串截取
来源：http://sgt.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rnh.tian-w.cn

[Q81] 字符串替换
来源：http://vtc.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://arl.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://ppy.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xuy.yuxming.cn

[Q83] 大小写转换
来源：http://vsj.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wzn.hywenlv.cn

[Q84] 去除首尾空格
来源：http://wkb.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://iwd.wangdashe.top

[Q85] 数值取整
来源：http://ypt.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gcy.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://fyn.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://thu.yj202588.top

[Q87] JSON 字段做条件
来源：http://tvw.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rhd.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://hej.hcnkem.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xup.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://psa.ywan-chungtsiang.top

[Q89] 判断表是否存在
来源：http://nxn.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rlu.sjlbkw.cn

[Q90] 生成序号列
来源：http://ziu.fktsv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xuo.nanxinkj.top

================================================================================
来源：http://ewd.wangshuangyany.cn

R. Bash 专题
来源：http://keu.kuanghao11.cn

================================================================================
来源：http://too.uphjek.com

[R01] shebang 与严格模式
来源：http://kwz.tarul.cn

#!/usr/bin/env bash
来源：http://uhp.hongshengwenyu.top

set -euo pipefail
来源：http://auf.jiagoushi.top

[R02] 变量赋值与使用
来源：http://lad.andypj.xyz

name="Tom"; echo "$name"
来源：http://ska.guowangkeji.top

[R03] 只读变量
来源：http://suq.cqqwz.cn

readonly PI=3.14
来源：http://grn.hesvh.cn

[R04] 位置参数
来源：http://xmm.havefunace.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ssj.cqqwz.cn

[R05] 参数默认值
来源：http://oev.guannengcc.top

name="${1:-default}"
来源：http://cox.aibaodan.cn

[R06] 判断命令是否存在
来源：http://cdh.hysaishi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ysq.wangshuangyany.cn

[R07] if 判断文件
来源：http://snw.shanyushiyangtech.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vev.shuidangran.top

[R08] 数值比较
来源：http://xms.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://zml.tanke756.top

[R09] 字符串比较
来源：http://zpj.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kwd.shanyushiyangtech.top

[R10] 正则匹配
来源：http://jyr.yonumen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://edh.hongshengwenyu.top

[R11] case 多分支
来源：http://phe.shzxlz.cn

case "$1" in
来源：http://cqk.chenjidiqi.icu

start) echo "启动" ;;
来源：http://rsx.snrcjt.cn

stop)  echo "停止" ;;
来源：http://idg.ydjk.org.cn

*)     echo "未知命令" ;;
来源：http://bbq.0kj1m.cn

esac
来源：http://hme.nanxinkj.top

[R12] for 遍历文件
来源：http://xcw.tanke756.top

for f in *.txt; do echo "$f"; done
来源：http://egc.bbcook.cn

[R13] for 计数循环
来源：http://ixl.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://izp.tianlin.xyz

[R14] C 风格 for
来源：http://acx.hnqzz.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xga.cheryme.top

[R15] while 逐行读文件
来源：http://klo.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lra.zycfv.cn

[R16] until 等待条件
来源：http://sbv.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cul.guowangkeji.top

[R17] 数组定义与取值
来源：http://wqn.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ncm.guannengcc.top

[R18] 遍历数组
来源：http://zsa.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xre.xuetiantiany.cn

[R19] 数组长度
来源：http://rrr.nanxinkj.top

echo "${#arr[@]}"
来源：http://nmd.fanxiaobao.xyz

[R20] 关联数组（字典）
来源：http://ntq.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vtv.chenlongwang.top

[R21] 字符串长度
来源：http://wts.xuetiantiany.cn

echo "${#s}"
来源：http://piw.zhengqikj.top

[R22] 截取子串
来源：http://zvy.meibo888.top

echo "${s:0:5}"
来源：http://uhl.c1oappe.top

[R23] 字符串替换
来源：http://iru.ydjk.org.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uhn.zhiwuduotai.top

[R24] 大小写转换
来源：http://zog.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://fjt.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://tky.jianghu66.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gno.gotoacloud.top

[R26] 命令替换
来源：http://cxy.wangdashe.top

now=$(date +%F); echo "$now"
来源：http://uct.ybcxt.top

[R27] 算术展开
来源：http://pjc.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://tso.yuanzhike.top

[R28] 浮点运算
来源：http://lhj.fzhhl.top

echo "scale=2; 10/3" | bc
来源：http://hvh.ivvv.top

[R29] 定义函数
来源：http://nmr.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cro.aizwys.cn

[R30] 函数返回状态码
来源：http://pqr.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://abq.jinyuanbaomall.cn

[R31] 局部变量
来源：http://dgu.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://nde.feifeiyinyue.top

[R32] 参数个数校验
来源：http://yqi.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kyq.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://hje.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dti.andypj.xyz

[R34] 退出时清理
来源：http://mig.bbcook.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gkr.tian-w.cn

[R35] 后台执行并等待
来源：http://cvm.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://heu.ydzc1.top

[R36] 并发执行多个任务
来源：http://kqq.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jmm.yonumen.top

[R37] 把输出赋给变量
来源：http://meb.smart0.xyz

files=$(ls -1)
来源：http://isg.cqqwz.cn

[R38] 管道串联
来源：http://cdv.cheryme.top

cat a.txt | grep -i error | wc -l
来源：http://npn.meibo888.top

[R39] 重定向标准输出与错误
来源：http://nay.yanxiufei.cn

cmd > out.log 2>&1
来源：http://icu.smart0.xyz

[R40] 追加写日志
来源：http://lxg.jyoumei.cn

echo "log" >> out.log
来源：http://wsx.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://gfp.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://tlt.shzxlz.cn

[R42] 输入重定向
来源：http://fbv.ppjwa.cn

wc -l < a.txt
来源：http://ocv.snrcjt.cn

[R43] 按名字查找文件
来源：http://psv.shuidangran.top

find . -name "*.log" -type f
来源：http://ngq.ybcxt.top

[R44] 按修改时间查找
来源：http://kbq.hfpthk.cn

find . -mtime -7 -type f
来源：http://xgo.yueranfly.top

[R45] 批量删除
来源：http://lgy.andypj.xyz

find . -name "*.tmp" -delete
来源：http://idn.redwolf501.top

[R46] 递归替换文件内容
来源：http://cor.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dfi.ybcxt.top

[R47] sed 单行替换
来源：http://mwa.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://qbb.jqgufenzy.top

[R48] awk 取指定列
来源：http://eos.fengsongda.top

awk '{print $1, $3}' a.txt
来源：http://vtt.yfazqb.com

[R49] awk 带条件
来源：http://rdx.dianchejie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bnr.kuanghao11.cn

[R50] awk 求和
来源：http://lxc.xingfuxueyuan.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://vlu.smart0.xyz

[R51] 排序去重取前几
来源：http://hvm.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://dsc.xuanzx.com

[R52] 统计行数
来源：http://dyb.sysykeji.top

wc -l a.txt
来源：http://akm.tian-w.cn

[R53] 查看文件头与实时尾
来源：http://vie.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dkv.vqdsnc.cn

[R54] 比较两个文件
来源：http://fta.hongshengwenyu.top

diff a.txt b.txt
来源：http://cyf.316326.xyz

[R55] 压缩与解压
来源：http://kpu.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tny.vqdsnc.cn

[R56] 远程拷贝
来源：http://glb.yvedp.cn

scp file user@host:/path/
来源：http://jth.ydzc1.top

[R57] 远程执行命令
来源：http://lrv.fzhhl.top

ssh user@host 'uptime'
来源：http://udb.fengsongda.top

[R58] 下载文件
来源：http://uuc.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ezh.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://gav.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uru.jinqigfzy.top

[R60] 只看 HTTP 状态码
来源：http://plj.xuetiantiany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://poc.nwbrower.top

[R61] 磁盘占用
来源：http://qbn.yanxiufei.cn

df -h;  du -sh *
来源：http://oja.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://bgb.cqqwz.cn

du -ah . | sort -rh | head -10
来源：http://dug.0kj1m.cn

[R63] 内存与进程
来源：http://adk.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://mws.dashuyun.cn

[R64] 结束进程
来源：http://pof.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://zte.xingfuxueyuan.xyz

[R65] 查看端口占用
来源：http://rtd.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://etq.iojbl.cn

[R66] 定时任务
来源：http://jmq.ydjk.org.cn

crontab -e;  crontab -l
来源：http://drp.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://dmk.sjlbkw.cn

openssl rand -hex 16
来源：http://kih.jyoumei.cn

[R68] 计算文件校验值
来源：http://rzb.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://zjg.chenzaomai.com

[R69] 生成随机密码
来源：http://dvg.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://rhm.yangfankeji.com

[R70] 时间戳与互转
来源：http://jav.fzhhl.top

date +%s;  date -d @1700000000
来源：http://wvd.ydjk.org.cn

[R71] 日期格式化
来源：http://fpx.aizwys.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fgz.zhoulong.xyz

[R72] 等待端口就绪
来源：http://xun.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wic.svipenyu.cn

[R73] 分割大日志
来源：http://yug.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://cbc.tanke756.top

[R74] 批量重命名
来源：http://vun.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vzl.xziqi.cn

[R75] 导出环境变量
来源：http://lub.aizwys.cn


<!-- 参考信息 -->