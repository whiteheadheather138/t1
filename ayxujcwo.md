代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://psi.jinqigfzy.top

[Q24] 去重
来源：http://jlu.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://vcp.yuanzhike.top

[Q25] 只取前 N 条
来源：http://lon.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lxs.nwbrower.top

[Q26] 计数
来源：http://hbk.daxiang520.top

SELECT COUNT(*) FROM users;
来源：http://sxt.tanke756.top

[Q27] 条件计数
来源：http://mdr.hnqzz.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rsv.wangshuangyany.cn

[Q28] 求和与平均
来源：http://mug.daxiang520.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fbg.hcnkem.com

[Q29] 最大最小值
来源：http://xgy.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zia.shanyushiyangtech.top

[Q30] 分组统计
来源：http://yje.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bsc.hywenlv.cn

[Q31] 分组后过滤
来源：http://cce.daria6918.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rdm.fengsongda.top

[Q32] 分组拼接字符串
来源：http://zog.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://foe.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zqp.yangfankeji.com

[Q33] 多列分组
来源：http://voq.pycfn.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ahr.ppjwa.cn

[Q34] 每组取第一条
来源：http://alp.chenlongwang.top

SELECT * FROM (
来源：http://qes.wangshuangyany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pdc.jiagoushi.top

) t WHERE rn = 1;
来源：http://rau.shuidangran.top

[Q35] 内连接
来源：http://wcv.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dox.ybcxt.top

[Q36] 左连接
来源：http://ofo.ctjpmb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qnf.0kj1m.cn

[Q37] 右连接
来源：http://jks.bjfxy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rsk.cqqwz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pee.nanxinkj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qvf.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://ecv.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://evx.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jhs.ywan-chungtsiang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hlo.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nqj.cdnleiting.top

[Q41] 多表连接
来源：http://hnh.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ook.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://bkk.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://bxb.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://ksm.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://pzt.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://arl.zhixingplan.top

[Q43] 标量子查询
来源：http://mkr.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wkl.svipenyu.cn

[Q44] IN 子查询
来源：http://fti.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ilz.bbcook.cn

[Q45] EXISTS 判断存在
来源：http://lob.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vwm.yueranfly.top

[Q46] NOT EXISTS 判断不存在
来源：http://rhj.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pvr.yueranfly.top

[Q47] 与平均值比较
来源：http://dtg.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fwj.jinghuilouyu.cn

[Q48] CTE 公用表表达式
来源：http://ixv.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://npf.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://wcb.iojbl.cn

[Q49] 更新单行
来源：http://qhq.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qza.snrcjt.cn

[Q50] 批量更新
来源：http://lfg.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fpg.zdqjudy.top

[Q51] 用子查询更新
来源：http://lpe.guannengcc.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wpc.zhoulong.xyz

[Q52] 删除指定行
来源：http://juy.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://rne.ctjpmb.com

[Q53] 按条件删除
来源：http://nsu.fehbvm.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://idz.bbcook.cn

[Q54] 清空表
来源：http://evx.chenzaomai.com

TRUNCATE TABLE logs;
来源：http://lrr.hcnkem.com

[Q55] 排名（并列占位）
来源：http://hgj.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://slx.feifeiyinyue.top

[Q56] 密集排名（并列不占位）
来源：http://uhl.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aiv.52xcode.cn

[Q57] 行号
来源：http://kdh.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tqy.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://bhb.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nds.fktsv.cn

[Q59] 分组内累计
来源：http://vfe.redwolf501.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://omk.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://haa.cucudq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bgl.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jgs.jyoumei.cn

[Q61] 移动平均
来源：http://cse.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wjq.gzhubu.top

[Q62] 分组占比
来源：http://ini.zdqjudy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pbf.chenjidiqi.icu

[Q63] 开启事务
来源：http://qff.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gby.ydjk.org.cn

[Q64] 提交事务
来源：http://fev.nanxuanxn.top

COMMIT;
来源：http://rfb.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://sfc.sufxvd.cn

ROLLBACK;
来源：http://ack.hnxiangtu.top

[Q66] 行锁查询
来源：http://qnk.jiagoushi.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mzx.bjfxy.top

[Q67] 设置隔离级别
来源：http://fwn.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tes.zhixingplan.top

[Q68] 保存点
来源：http://hpa.bjfxy.top

SAVEPOINT sp1;
来源：http://pqc.nwbrower.top

ROLLBACK TO sp1;
来源：http://inh.cashguo.top

[Q69] 查看执行计划
来源：http://tdm.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tcj.yj20258888.top

[Q70] 更新统计信息
来源：http://vin.yj20258888.top

ANALYZE TABLE users;
来源：http://fnk.uphjek.com

[Q71] 查看建表语句
来源：http://psy.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xwe.pycfn.com

[Q72] 查看索引
来源：http://gei.nanxinkj.top

SHOW INDEX FROM users;
来源：http://xvh.iojbl.cn

[Q73] 查看表状态
来源：http://svm.hcnkem.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ghl.gogol.net.cn

[Q74] 强制使用索引
来源：http://qui.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jyx.316326.xyz

[Q75] 日期格式化
来源：http://hts.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nqh.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ibo.0kj1m.cn

[Q76] 按天统计
来源：http://nmd.yfazqb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xln.shangyingyoupin.top

[Q77] 时间加减
来源：http://xjq.ybcxt.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jwu.zhiwuduotai.top

[Q78] 当前时间
来源：http://jrz.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gsb.gogol.net.cn

[Q79] 字符串拼接
来源：http://guj.cqqwz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aby.yj20258888.top

[Q80] 字符串截取
来源：http://pty.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lmf.sweek.top

[Q81] 字符串替换
来源：http://ghs.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cbl.xingfuxueyuan.xyz

[Q82] 字符长度与字节长度
来源：http://mkk.hcnkem.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uzh.hywenlv.cn

[Q83] 大小写转换
来源：http://ozm.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wry.yvedp.cn

[Q84] 去除首尾空格
来源：http://ewj.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://msp.sysykeji.top

[Q85] 数值取整
来源：http://ymk.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://swf.jlsjyb.cn

[Q86] 读取 JSON 字段
来源：http://fbv.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://npx.cqqwz.cn

[Q87] JSON 字段做条件
来源：http://fyg.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ojo.hongshengwenyu.top

[Q88] 行转列（条件聚合）
来源：http://tef.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oft.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://not.xuanzx.com

[Q89] 判断表是否存在
来源：http://kps.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qmi.xuetiantiany.cn

[Q90] 生成序号列
来源：http://rtp.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ihg.daxiang520.top

================================================================================
来源：http://mzd.gotoacloud.top

R. Bash 专题
来源：http://vtw.ehwqpu.com

================================================================================
来源：http://bdr.shangyingyoupin.top

[R01] shebang 与严格模式
来源：http://con.haohaochexian.top

#!/usr/bin/env bash
来源：http://wrl.zdqjudy.top

set -euo pipefail
来源：http://qbv.nanxinkj.top

[R02] 变量赋值与使用
来源：http://loa.cheryme.top

name="Tom"; echo "$name"
来源：http://mvg.ywan-chungtsiang.top

[R03] 只读变量
来源：http://lof.dianchejie.cn

readonly PI=3.14
来源：http://mwq.fengsongda.top

[R04] 位置参数
来源：http://myl.ydjk.org.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qrc.tarul.cn

[R05] 参数默认值
来源：http://khw.hnqzz.top

name="${1:-default}"
来源：http://udp.ydzc1.top

[R06] 判断命令是否存在
来源：http://set.hysaishi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cgq.hammf.cn

[R07] if 判断文件
来源：http://jps.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eln.meibo888.top

[R08] 数值比较
来源：http://zbu.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://ogy.gogol.net.cn

[R09] 字符串比较
来源：http://txz.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ibz.9152youxi.cn

[R10] 正则匹配
来源：http://qnq.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rcg.ctjpmb.com

[R11] case 多分支
来源：http://kkj.zhijiandao.cn

case "$1" in
来源：http://gfq.ybcxt.top

start) echo "启动" ;;
来源：http://nkd.yongpay.top

stop)  echo "停止" ;;
来源：http://rxj.bbcook.cn

*)     echo "未知命令" ;;
来源：http://cbq.chenlongwang.top

esac
来源：http://hvu.meibo888.top

[R12] for 遍历文件
来源：http://iln.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://hcc.xuanzx.com

[R13] for 计数循环
来源：http://hsy.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://vyi.meibo888.top

[R14] C 风格 for
来源：http://rhj.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mnc.yj20258.top

[R15] while 逐行读文件
来源：http://wzt.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lcv.yongpay.top

[R16] until 等待条件
来源：http://kgk.9152youxi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qng.vqdsnc.cn

[R17] 数组定义与取值
来源：http://bog.aizwys.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dcf.zhaomingkeji.xyz

[R18] 遍历数组
来源：http://ovz.9152youxi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://enf.9152youxi.cn

[R19] 数组长度
来源：http://fcc.ppjwa.cn

echo "${#arr[@]}"
来源：http://avc.tanke756.top

[R20] 关联数组（字典）
来源：http://szq.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://reb.smart0.xyz

[R21] 字符串长度
来源：http://bfn.jinyuanbaomall.cn

echo "${#s}"
来源：http://jsy.9152youxi.cn

[R22] 截取子串
来源：http://vxb.hammf.cn

echo "${s:0:5}"
来源：http://jwd.quarkkingdee.top

[R23] 字符串替换
来源：http://cfl.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sxj.fanxiaobao.xyz

[R24] 大小写转换
来源：http://jua.ydjk.org.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ikv.52xcode.cn

[R25] 去后缀 / 去前缀
来源：http://haz.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gtq.guannengcc.top

[R26] 命令替换
来源：http://klc.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://uep.shanyushiyangkeji.top

[R27] 算术展开
来源：http://wpm.yonumen.top

echo $((1 + 2 * 3))
来源：http://ldw.gogol.net.cn

[R28] 浮点运算
来源：http://nvl.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://luu.316326.xyz

[R29] 定义函数
来源：http://amq.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cso.hysaishi.cn

[R30] 函数返回状态码
来源：http://lwy.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://scu.ivvv.top

[R31] 局部变量
来源：http://wda.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://bgt.sweek.top

[R32] 参数个数校验
来源：http://ujp.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yrt.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://eca.chenzaomai.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://msz.yj20258888.top

[R34] 退出时清理
来源：http://whs.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://ryo.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://pwe.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fjm.zycfv.cn

[R36] 并发执行多个任务
来源：http://fcf.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://phq.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://vxh.hongshengwenyu.top

files=$(ls -1)
来源：http://bzi.pengpengdd.cyou

[R38] 管道串联
来源：http://oxs.jqgfzy.top

cat a.txt | grep -i error | wc -l
来源：http://beo.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://kjf.yanxiufei.cn

cmd > out.log 2>&1
来源：http://ttn.bjfxy.top

[R40] 追加写日志
来源：http://tkc.yj20258888.top

echo "log" >> out.log
来源：http://jxi.ybcxt.top

[R41] 丢弃输出
来源：http://hnx.cheryme.top

cmd >/dev/null 2>&1
来源：http://ims.cashguo.top

[R42] 输入重定向
来源：http://lhf.cheryme.top

wc -l < a.txt
来源：http://mvf.zhijiandao.cn

[R43] 按名字查找文件
来源：http://qjp.ehwqpu.com

find . -name "*.log" -type f
来源：http://syc.meibo888.top

[R44] 按修改时间查找
来源：http://zty.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://wrk.zhiwuduotai.top

[R45] 批量删除
来源：http://ire.yongpay.top

find . -name "*.tmp" -delete
来源：http://xay.ehwqpu.com

[R46] 递归替换文件内容
来源：http://bto.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lya.tarul.cn

[R47] sed 单行替换
来源：http://kib.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://nwt.xuanzx.com

[R48] awk 取指定列
来源：http://lpw.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://hzq.jqgufenzy.top

[R49] awk 带条件
来源：http://tdh.fehbvm.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tnv.0kj1m.cn

[R50] awk 求和
来源：http://rxn.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://cjj.tianlin.xyz

[R51] 排序去重取前几
来源：http://ehc.zhongyouzk.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ode.uphjek.com

[R52] 统计行数
来源：http://jtd.zdqjudy.top

wc -l a.txt
来源：http://ovg.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://qqb.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zmz.uphjek.com

[R54] 比较两个文件
来源：http://bij.yangfankeji.com

diff a.txt b.txt
来源：http://smn.sufxvd.cn

[R55] 压缩与解压
来源：http://rtm.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xdu.yuanzhike.top

[R56] 远程拷贝
来源：http://wkr.zdbjq.cn

scp file user@host:/path/
来源：http://abx.pycfn.com

[R57] 远程执行命令
来源：http://lry.svipenyu.cn

ssh user@host 'uptime'
来源：http://dcg.feifeiyinyue.top

[R58] 下载文件
来源：http://sqs.0kj1m.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tlp.0kj1m.cn

[R59] 发 POST JSON
来源：http://vkn.xziqi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jmj.ehwqpu.com

[R60] 只看 HTTP 状态码
来源：http://wij.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fpm.cdnleiting.top

[R61] 磁盘占用
来源：http://tkd.sxryk.cn

df -h;  du -sh *
来源：http://iru.shzxlz.cn

[R62] 找最占空间的文件
来源：http://pge.hammf.cn

du -ah . | sort -rh | head -10
来源：http://sro.yangfankeji.com

[R63] 内存与进程
来源：http://bhx.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://yku.ehwqpu.com

[R64] 结束进程
来源：http://uds.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://ajv.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://rxu.meibo888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cdn.dianchejie.cn

[R66] 定时任务
来源：http://jiq.xingfuxueyuan.xyz

crontab -e;  crontab -l
来源：http://drs.ydzc1.top

[R67] 生成随机十六进制串
来源：http://mwk.chenjidiqi.icu

openssl rand -hex 16
来源：http://ciz.hesvh.cn

[R68] 计算文件校验值
来源：http://ccx.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pwx.iojbl.cn

[R69] 生成随机密码
来源：http://hiw.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://azo.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://cqv.yj20258.top

date +%s;  date -d @1700000000
来源：http://ioo.haohaochexian.top

[R71] 日期格式化
来源：http://csg.hcnkem.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://pyb.yvedp.cn

[R72] 等待端口就绪
来源：http://dep.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bpq.jqgfzy.top

[R73] 分割大日志
来源：http://byh.0kj1m.cn


<!-- 参考信息 -->