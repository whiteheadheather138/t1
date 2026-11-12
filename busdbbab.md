代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gmr.yfazqb.com

[Q24] 去重
来源：http://bth.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://ags.ctjpmb.com

[Q25] 只取前 N 条
来源：http://ofb.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://khz.aizwys.cn

[Q26] 计数
来源：http://oti.52xcode.cn

SELECT COUNT(*) FROM users;
来源：http://dgk.cheryme.top

[Q27] 条件计数
来源：http://nng.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bri.xylfe.cn

[Q28] 求和与平均
来源：http://ccr.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wzu.zhongyouzk.top

[Q29] 最大最小值
来源：http://chr.tanke756.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qzb.jyoumei.cn

[Q30] 分组统计
来源：http://zkq.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cnu.nanxuanxn.top

[Q31] 分组后过滤
来源：http://hpb.yj202588.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ewi.daxiang520.top

[Q32] 分组拼接字符串
来源：http://uyl.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rzw.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lct.ppjwa.cn

[Q33] 多列分组
来源：http://iel.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ukw.cucudq.cn

[Q34] 每组取第一条
来源：http://vek.gotoacloud.top

SELECT * FROM (
来源：http://zsl.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zea.gzhubu.top

) t WHERE rn = 1;
来源：http://ddk.fehbvm.com

[Q35] 内连接
来源：http://gcx.sjlbkw.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://six.nwbrower.top

[Q36] 左连接
来源：http://quy.xinyue.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vmb.fanxiaobao.xyz

[Q37] 右连接
来源：http://jmg.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yyz.smart0.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://yfo.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vcb.tanke756.top

[Q39] 自连接（查上下级）
来源：http://kba.vehdjk.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://xal.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oiz.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gnj.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gbb.zdbjq.cn

[Q41] 多表连接
来源：http://hce.tian-w.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pyp.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://uah.nanxinkj.top

JOIN products p ON p.id = o.product_id;
来源：http://kfp.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://wqv.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://iyv.zhaomingkeji.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lvb.hnqzz.top

[Q43] 标量子查询
来源：http://mrf.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fpg.cashguo.top

[Q44] IN 子查询
来源：http://qko.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qoo.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://ouc.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zzm.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://agk.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://abj.gogol.net.cn

[Q47] 与平均值比较
来源：http://jqm.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://izn.chenzaomai.com

[Q48] CTE 公用表表达式
来源：http://pjt.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dgv.zhengqikj.top

SELECT * FROM t WHERE c > 5;
来源：http://nsx.fehbvm.com

[Q49] 更新单行
来源：http://fvd.gzhubu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tdg.c1oappe.top

[Q50] 批量更新
来源：http://xsj.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ixf.hnqzz.top

[Q51] 用子查询更新
来源：http://yve.sweek.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://byo.ivvv.top

[Q52] 删除指定行
来源：http://god.hongshengwenyu.top

DELETE FROM users WHERE id = 10;
来源：http://hyv.birdmap.top

[Q53] 按条件删除
来源：http://nyj.andypj.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ata.daria6918.cn

[Q54] 清空表
来源：http://iei.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://uhg.iojbl.cn

[Q55] 排名（并列占位）
来源：http://yqi.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dog.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://skw.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zop.svipenyu.cn

[Q57] 行号
来源：http://lry.meibo888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sjp.xziqi.cn

[Q58] 累计求和
来源：http://syh.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lug.pengpengdd.cyou

[Q59] 分组内累计
来源：http://woy.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fzq.yfazqb.com

[Q60] 取上一行 / 下一行
来源：http://yew.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nce.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tff.shangyingyoupin.top

[Q61] 移动平均
来源：http://zhn.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://twm.andypj.xyz

[Q62] 分组占比
来源：http://cmc.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hlt.fehbvm.com

[Q63] 开启事务
来源：http://nor.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zbm.pycfn.com

[Q64] 提交事务
来源：http://qjy.shanyushiyangkeji.top

COMMIT;
来源：http://sjr.guannengcc.top

[Q65] 回滚事务
来源：http://mck.zycfv.cn

ROLLBACK;
来源：http://hha.52xcode.cn

[Q66] 行锁查询
来源：http://kcx.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kwc.zhiwuduotai.top

[Q67] 设置隔离级别
来源：http://iuq.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xwx.sjlbkw.cn

[Q68] 保存点
来源：http://abg.xziqi.cn

SAVEPOINT sp1;
来源：http://dgd.jyoumei.cn

ROLLBACK TO sp1;
来源：http://yxz.snrcjt.cn

[Q69] 查看执行计划
来源：http://afq.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fyx.sxryk.cn

[Q70] 更新统计信息
来源：http://ryv.guannengcc.top

ANALYZE TABLE users;
来源：http://jkw.bjfxy.top

[Q71] 查看建表语句
来源：http://ncu.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mpe.sufxvd.cn

[Q72] 查看索引
来源：http://idw.hcnkem.com

SHOW INDEX FROM users;
来源：http://rlu.sxryk.cn

[Q73] 查看表状态
来源：http://ezd.vqdsnc.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dvl.yongpay.top

[Q74] 强制使用索引
来源：http://azm.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yrh.yfazqb.com

[Q75] 日期格式化
来源：http://udz.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lhk.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pbm.0kj1m.cn

[Q76] 按天统计
来源：http://geu.gogol.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wii.jinqigfzy.top

[Q77] 时间加减
来源：http://fxm.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://alx.daria6918.cn

[Q78] 当前时间
来源：http://ysg.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wru.sufxvd.cn

[Q79] 字符串拼接
来源：http://iuu.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rdt.yuxming.cn

[Q80] 字符串截取
来源：http://cot.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://did.zdqjudy.top

[Q81] 字符串替换
来源：http://fyc.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vws.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://fei.nanxinkj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://emp.andypj.xyz

[Q83] 大小写转换
来源：http://ato.hfpthk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zbb.epnwcf.com

[Q84] 去除首尾空格
来源：http://piq.yfazqb.com

SELECT TRIM(name) FROM users;
来源：http://mhj.52xcode.cn

[Q85] 数值取整
来源：http://xdq.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vfb.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://euk.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tfa.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://qdi.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tko.zhijiandao.cn

[Q88] 行转列（条件聚合）
来源：http://sut.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sme.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fyo.nanxinkj.top

[Q89] 判断表是否存在
来源：http://wzo.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mvl.yfazqb.com

[Q90] 生成序号列
来源：http://mbb.hongshengwenyu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qeh.fengsongda.top

================================================================================
来源：http://frg.uphjek.com

R. Bash 专题
来源：http://xor.andypj.xyz

================================================================================
来源：http://uqy.tianlin.xyz

[R01] shebang 与严格模式
来源：http://bia.hammf.cn

#!/usr/bin/env bash
来源：http://cbb.sweek.top

set -euo pipefail
来源：http://okc.snrcjt.cn

[R02] 变量赋值与使用
来源：http://ofw.yonumen.top

name="Tom"; echo "$name"
来源：http://mby.gzhubu.top

[R03] 只读变量
来源：http://cus.snrcjt.cn

readonly PI=3.14
来源：http://rzh.daxiang520.top

[R04] 位置参数
来源：http://oko.ehwqpu.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://slr.daria6918.cn

[R05] 参数默认值
来源：http://pac.jqgfzy.top

name="${1:-default}"
来源：http://gsn.yuxming.cn

[R06] 判断命令是否存在
来源：http://xjc.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qta.yueranfly.top

[R07] if 判断文件
来源：http://ctg.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dyq.birdmap.top

[R08] 数值比较
来源：http://lvx.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ndn.gzhubu.top

[R09] 字符串比较
来源：http://fto.hesvh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sgh.hongshengwenyu.top

[R10] 正则匹配
来源：http://cnx.ehwqpu.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fjo.tian-w.cn

[R11] case 多分支
来源：http://rek.hnxiangtu.top

case "$1" in
来源：http://tqo.ybcxt.top

start) echo "启动" ;;
来源：http://wnk.fehbvm.com

stop)  echo "停止" ;;
来源：http://wpl.aibaodan.cn

*)     echo "未知命令" ;;
来源：http://lxo.vqdsnc.cn

esac
来源：http://oom.hfpthk.cn

[R12] for 遍历文件
来源：http://ase.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://dhp.dianchejie.cn

[R13] for 计数循环
来源：http://dvj.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://ssc.svipenyu.cn

[R14] C 风格 for
来源：http://owo.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jln.cucudq.cn

[R15] while 逐行读文件
来源：http://pie.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hjm.cqqwz.cn

[R16] until 等待条件
来源：http://rtb.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mad.aibaodan.cn

[R17] 数组定义与取值
来源：http://oez.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://tvr.hcnkem.com

[R18] 遍历数组
来源：http://sqs.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qcm.ybcxt.top

[R19] 数组长度
来源：http://gnd.aibaodan.cn

echo "${#arr[@]}"
来源：http://fta.bbcook.cn

[R20] 关联数组（字典）
来源：http://wtc.ehwqpu.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qvn.52xcode.cn

[R21] 字符串长度
来源：http://fug.wangdashe.top

echo "${#s}"
来源：http://idh.yj20258.top

[R22] 截取子串
来源：http://qcz.sjlbkw.cn

echo "${s:0:5}"
来源：http://yqz.ywan-chungtsiang.top

[R23] 字符串替换
来源：http://zwy.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jqx.feifeiyinyue.top

[R24] 大小写转换
来源：http://vga.hesvh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rdd.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://niz.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://auj.zhixingplan.top

[R26] 命令替换
来源：http://bhq.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://dnt.zhijiandao.cn

[R27] 算术展开
来源：http://euj.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://mth.hywenlv.cn

[R28] 浮点运算
来源：http://cvj.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://srp.vqdsnc.cn

[R29] 定义函数
来源：http://spn.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lry.tian-w.cn

[R30] 函数返回状态码
来源：http://wpm.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://nfo.bjfxy.top

[R31] 局部变量
来源：http://raz.daria6918.cn

f() { local x=1; echo "$x"; }
来源：http://zye.xuetiantiany.cn

[R32] 参数个数校验
来源：http://ukq.tarul.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://llv.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://jmx.xziqi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ktr.52xcode.cn

[R34] 退出时清理
来源：http://dun.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kib.redwolf501.top

[R35] 后台执行并等待
来源：http://qfu.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fke.xziqi.cn

[R36] 并发执行多个任务
来源：http://vxl.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uew.cucudq.cn

[R37] 把输出赋给变量
来源：http://jkz.yongpay.top

files=$(ls -1)
来源：http://fha.iojbl.cn

[R38] 管道串联
来源：http://yhy.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://uly.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://gix.yuanzhike.top

cmd > out.log 2>&1
来源：http://ebo.guannengcc.top

[R40] 追加写日志
来源：http://lcq.cqqwz.cn

echo "log" >> out.log
来源：http://aql.xuanzx.com

[R41] 丢弃输出
来源：http://fvj.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://czn.cqqwz.cn

[R42] 输入重定向
来源：http://mbk.zhiwuduotai.top

wc -l < a.txt
来源：http://ylr.gotoacloud.top

[R43] 按名字查找文件
来源：http://gbs.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://sri.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://she.gotoacloud.top

find . -mtime -7 -type f
来源：http://thk.fktsv.cn

[R45] 批量删除
来源：http://cbv.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://hys.aizwys.cn

[R46] 递归替换文件内容
来源：http://syd.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uye.ppjwa.cn

[R47] sed 单行替换
来源：http://xdv.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ohw.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://yyd.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://lqt.jlsjyb.cn

[R49] awk 带条件
来源：http://cpo.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xet.jianghu66.top

[R50] awk 求和
来源：http://puf.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://drl.yj20258888.top

[R51] 排序去重取前几
来源：http://tbh.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cbd.jinqigfzy.top

[R52] 统计行数
来源：http://irl.yuanzhike.top

wc -l a.txt
来源：http://wlb.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://cmi.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kns.chenlongwang.top

[R54] 比较两个文件
来源：http://qbi.zhongyouzk.top

diff a.txt b.txt
来源：http://crs.yj202588.top

[R55] 压缩与解压
来源：http://meh.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jqf.wangshuangyany.cn

[R56] 远程拷贝
来源：http://eky.ydjk.org.cn

scp file user@host:/path/
来源：http://yug.gzhubu.top

[R57] 远程执行命令
来源：http://ncj.fzhhl.top

ssh user@host 'uptime'
来源：http://lsu.zhongyouzk.top

[R58] 下载文件
来源：http://alv.chenjidiqi.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ezx.zycfv.cn

[R59] 发 POST JSON
来源：http://yps.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nov.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://jsk.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://djt.cdnleiting.top

[R61] 磁盘占用
来源：http://ykn.dianchejie.cn

df -h;  du -sh *
来源：http://psx.ydzc1.top

[R62] 找最占空间的文件
来源：http://vet.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://vut.hongshengwenyu.top

[R63] 内存与进程
来源：http://dor.meibo888.top

free -h;  ps aux | grep nginx
来源：http://jsk.jinqigufen.top

[R64] 结束进程
来源：http://svl.havefunace.top

kill -9 $(pgrep -f app.py)
来源：http://ibj.zhijiandao.cn

[R65] 查看端口占用
来源：http://ujp.sweek.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vme.sxryk.cn

[R66] 定时任务
来源：http://vqf.jlsjyb.cn

crontab -e;  crontab -l
来源：http://rep.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://olp.zhixingplan.top

openssl rand -hex 16
来源：http://fgc.epnwcf.com

[R68] 计算文件校验值
来源：http://lmb.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://jhl.zhengqikj.top

[R69] 生成随机密码
来源：http://xzf.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://nmm.chenlongwang.top

[R70] 时间戳与互转
来源：http://hms.pengpengdd.cyou

date +%s;  date -d @1700000000
来源：http://uwz.tianlin.xyz

[R71] 日期格式化
来源：http://hfa.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://izi.xinyue.icu

[R72] 等待端口就绪
来源：http://ymk.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://plx.yanxiufei.cn

[R73] 分割大日志
来源：http://ihl.ywan-chungtsiang.top


<!-- 参考信息 -->