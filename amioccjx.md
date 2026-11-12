代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xcq.haohaochexian.top

[Q28] 求和与平均
来源：http://tvx.tarul.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ran.ivvv.top

[Q29] 最大最小值
来源：http://iyf.cqqwz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oan.zycfv.cn

[Q30] 分组统计
来源：http://ezf.tarul.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://efo.yueranfly.top

[Q31] 分组后过滤
来源：http://koi.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ifz.nanxinkj.top

[Q32] 分组拼接字符串
来源：http://egq.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dgc.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mtp.tianlin.xyz

[Q33] 多列分组
来源：http://kin.aizwys.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lex.ydzc1.top

[Q34] 每组取第一条
来源：http://fez.9152youxi.cn

SELECT * FROM (
来源：http://euk.xinyue.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sqi.hnxiangtu.top

) t WHERE rn = 1;
来源：http://zgk.cqqwz.cn

[Q35] 内连接
来源：http://zve.zdbjq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bnq.yueranfly.top

[Q36] 左连接
来源：http://ika.jlsjyb.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://irg.zdqjudy.top

[Q37] 右连接
来源：http://rul.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lob.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://wkk.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://seb.yj202588.top

[Q39] 自连接（查上下级）
来源：http://kjv.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://big.epnwcf.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eyn.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://oae.xinyue.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dwh.nanxinkj.top

[Q41] 多表连接
来源：http://dsv.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rss.bbcook.cn

JOIN users u ON u.id = o.user_id
来源：http://azg.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://qzf.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://mao.hammf.cn

SELECT u.name, o.amount FROM users u
来源：http://vwe.guannengcc.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://afk.hnxiangtu.top

[Q43] 标量子查询
来源：http://atb.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://laa.dashuyun.cn

[Q44] IN 子查询
来源：http://xfv.hysaishi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ukh.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://mzc.gzhubu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://upg.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://nor.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ini.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://sol.fzhhl.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lcl.yuxming.cn

[Q48] CTE 公用表表达式
来源：http://xbd.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lrg.tianlin.xyz

SELECT * FROM t WHERE c > 5;
来源：http://izb.yj20258.top

[Q49] 更新单行
来源：http://ood.fzhhl.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hni.daria6918.cn

[Q50] 批量更新
来源：http://szk.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cfy.fengsongda.top

[Q51] 用子查询更新
来源：http://gtl.yangfankeji.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eyq.hnxiangtu.top

[Q52] 删除指定行
来源：http://gsq.cashguo.top

DELETE FROM users WHERE id = 10;
来源：http://ufk.jinqigfzy.top

[Q53] 按条件删除
来源：http://qkd.uphjek.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://obm.cheryme.top

[Q54] 清空表
来源：http://ukt.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://bcq.sweek.top

[Q55] 排名（并列占位）
来源：http://aqs.haohaochexian.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://soy.fanxiaobao.xyz

[Q56] 密集排名（并列不占位）
来源：http://pld.ivvv.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://des.yangfankeji.com

[Q57] 行号
来源：http://otc.cashguo.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zsd.chenjidiqi.icu

[Q58] 累计求和
来源：http://hjy.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jpm.snrcjt.cn

[Q59] 分组内累计
来源：http://ftu.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pqo.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://ocv.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hfh.redwolf501.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bix.jinqigfzy.top

[Q61] 移动平均
来源：http://wem.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uma.zhixingplan.top

[Q62] 分组占比
来源：http://mau.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pzr.hammf.cn

[Q63] 开启事务
来源：http://otp.nwbrower.top

START TRANSACTION;                -- 或 BEGIN
来源：http://coq.daria6918.cn

[Q64] 提交事务
来源：http://bks.hesvh.cn

COMMIT;
来源：http://iuf.smart0.xyz

[Q65] 回滚事务
来源：http://igu.quarkkingdee.top

ROLLBACK;
来源：http://mxr.tianlin.xyz

[Q66] 行锁查询
来源：http://zaf.jianghu66.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dwe.epnwcf.com

[Q67] 设置隔离级别
来源：http://wll.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oif.bbcook.cn

[Q68] 保存点
来源：http://hef.tarul.cn

SAVEPOINT sp1;
来源：http://xvo.yuxming.cn

ROLLBACK TO sp1;
来源：http://ria.xinyue.icu

[Q69] 查看执行计划
来源：http://zah.yfazqb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xhs.ctjpmb.com

[Q70] 更新统计信息
来源：http://quv.sufxvd.cn

ANALYZE TABLE users;
来源：http://hix.yongpay.top

[Q71] 查看建表语句
来源：http://cra.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yqu.sweek.top

[Q72] 查看索引
来源：http://ran.quarkkingdee.top

SHOW INDEX FROM users;
来源：http://fxx.birdmap.top

[Q73] 查看表状态
来源：http://lqt.jqgfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uhp.yangfankeji.com

[Q74] 强制使用索引
来源：http://bhz.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://twz.bjfxy.top

[Q75] 日期格式化
来源：http://caa.jianghu66.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wil.kuanghao11.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zkd.316326.xyz

[Q76] 按天统计
来源：http://hrg.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mcx.cqqwz.cn

[Q77] 时间加减
来源：http://ktv.xziqi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cvl.cdnleiting.top

[Q78] 当前时间
来源：http://fkc.jianghu66.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://trz.jinqigfzy.top

[Q79] 字符串拼接
来源：http://stc.yvedp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://olr.svipenyu.cn

[Q80] 字符串截取
来源：http://iva.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://znf.ehwqpu.com

[Q81] 字符串替换
来源：http://qfq.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rzf.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://irz.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jmb.yuanzhike.top

[Q83] 大小写转换
来源：http://aqo.zhiwuduotai.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hjr.hywenlv.cn

[Q84] 去除首尾空格
来源：http://qab.daria6918.cn

SELECT TRIM(name) FROM users;
来源：http://cxf.ydjk.org.cn

[Q85] 数值取整
来源：http://klz.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wma.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://axg.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://afi.havefunace.top

[Q87] JSON 字段做条件
来源：http://dot.cashguo.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bsj.cqqwz.cn

[Q88] 行转列（条件聚合）
来源：http://ktd.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jhk.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wir.havefunace.top

[Q89] 判断表是否存在
来源：http://alh.quarkkingdee.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://aad.9152youxi.cn

[Q90] 生成序号列
来源：http://num.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pmx.zhiwuduotai.top

================================================================================
来源：http://jhd.hongshengwenyu.top

R. Bash 专题
来源：http://gts.gzhubu.top

================================================================================
来源：http://fjp.ehwqpu.com

[R01] shebang 与严格模式
来源：http://gtt.fehbvm.com

#!/usr/bin/env bash
来源：http://xzn.tian-w.cn

set -euo pipefail
来源：http://azh.jianghu66.top

[R02] 变量赋值与使用
来源：http://onc.jyoumei.cn

name="Tom"; echo "$name"
来源：http://otz.jqgufenzy.top

[R03] 只读变量
来源：http://rmn.vqdsnc.cn

readonly PI=3.14
来源：http://vfv.snrcjt.cn

[R04] 位置参数
来源：http://vrl.wangshuangyany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bdj.hammf.cn

[R05] 参数默认值
来源：http://occ.wangshuangyany.cn

name="${1:-default}"
来源：http://drr.yanxiufei.cn

[R06] 判断命令是否存在
来源：http://gtw.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hbr.jinqigfzy.top

[R07] if 判断文件
来源：http://njg.ywan-chungtsiang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://skq.gogol.net.cn

[R08] 数值比较
来源：http://xdh.zhiwuduotai.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uyc.jianghu66.top

[R09] 字符串比较
来源：http://jfn.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ydv.yangfankeji.com

[R10] 正则匹配
来源：http://mme.snrcjt.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ang.0kj1m.cn

[R11] case 多分支
来源：http://glw.zhengqikj.top

case "$1" in
来源：http://xcn.fktsv.cn

start) echo "启动" ;;
来源：http://mfs.zhijiandao.cn

stop)  echo "停止" ;;
来源：http://oaj.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://igr.jianghu66.top

esac
来源：http://uea.ydjk.org.cn

[R12] for 遍历文件
来源：http://svs.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://kpg.zdqjudy.top

[R13] for 计数循环
来源：http://jhg.ehwqpu.com

for i in {1..10}; do echo "$i"; done
来源：http://yyl.gotoacloud.top

[R14] C 风格 for
来源：http://xls.yonumen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hld.bbcook.cn

[R15] while 逐行读文件
来源：http://rfl.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://api.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://msq.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://plw.zdbjq.cn

[R17] 数组定义与取值
来源：http://gks.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://csx.xinyue.icu

[R18] 遍历数组
来源：http://psy.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rnk.daria6918.cn

[R19] 数组长度
来源：http://zcj.mhx1999.top

echo "${#arr[@]}"
来源：http://gyz.sysykeji.top

[R20] 关联数组（字典）
来源：http://huk.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hwo.redwolf501.top

[R21] 字符串长度
来源：http://puk.nanxuanxn.top

echo "${#s}"
来源：http://ixl.wangshuangyany.cn

[R22] 截取子串
来源：http://bmf.xinyue.icu

echo "${s:0:5}"
来源：http://ryg.xziqi.cn

[R23] 字符串替换
来源：http://wmr.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qlf.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://aol.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://loo.hnxiangtu.top

[R25] 去后缀 / 去前缀
来源：http://zfs.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zro.c1oappe.top

[R26] 命令替换
来源：http://egw.zhijiandao.cn

now=$(date +%F); echo "$now"
来源：http://rkj.bbcook.cn

[R27] 算术展开
来源：http://bhx.uphjek.com

echo $((1 + 2 * 3))
来源：http://rbd.hnqzz.top

[R28] 浮点运算
来源：http://rog.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://lhr.shuidangran.top

[R29] 定义函数
来源：http://jha.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yfo.guannengcc.top

[R30] 函数返回状态码
来源：http://zhs.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://fdw.sjlbkw.cn

[R31] 局部变量
来源：http://mjq.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://nzv.yj202588.top

[R32] 参数个数校验
来源：http://kbt.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ptb.jinqigfzy.top

[R33] 捕获错误并提示行号
来源：http://sqe.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://llb.xziqi.cn

[R34] 退出时清理
来源：http://foa.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://yvi.zycfv.cn

[R35] 后台执行并等待
来源：http://xno.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ppq.snrcjt.cn

[R36] 并发执行多个任务
来源：http://qsb.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ifm.nwbrower.top

[R37] 把输出赋给变量
来源：http://pcq.ywan-chungtsiang.top

files=$(ls -1)
来源：http://wfs.ydjk.org.cn

[R38] 管道串联
来源：http://qvx.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://lwb.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://raj.hnxiangtu.top

cmd > out.log 2>&1
来源：http://nez.jinqigfzy.top

[R40] 追加写日志
来源：http://tag.chenjidiqi.icu

echo "log" >> out.log
来源：http://jxo.bjfxy.top

[R41] 丢弃输出
来源：http://gcf.jqgufenzy.top

cmd >/dev/null 2>&1
来源：http://ylf.ydjk.org.cn

[R42] 输入重定向
来源：http://qbg.fzhhl.top

wc -l < a.txt
来源：http://yvz.sxryk.cn

[R43] 按名字查找文件
来源：http://tiy.nanxinkj.top

find . -name "*.log" -type f
来源：http://vxj.ehwqpu.com

[R44] 按修改时间查找
来源：http://nyu.gzhubu.top

find . -mtime -7 -type f
来源：http://kkd.zhiwuduotai.top

[R45] 批量删除
来源：http://hdu.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://gmh.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://wwc.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://far.hywenlv.cn

[R47] sed 单行替换
来源：http://sad.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://ash.xylfe.cn

[R48] awk 取指定列
来源：http://bwu.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://vrn.zdqjudy.top

[R49] awk 带条件
来源：http://zru.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ddm.jqgufenzy.top

[R50] awk 求和
来源：http://vxi.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://scc.tanke756.top

[R51] 排序去重取前几
来源：http://adq.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gls.iojbl.cn

[R52] 统计行数
来源：http://nzp.shanyushiyangtech.top

wc -l a.txt
来源：http://gxq.hammf.cn

[R53] 查看文件头与实时尾
来源：http://waf.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://chn.jqgufenzy.top

[R54] 比较两个文件
来源：http://hlm.nanxuanxn.top

diff a.txt b.txt
来源：http://hyk.fzhhl.top

[R55] 压缩与解压
来源：http://rwk.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ibu.ctjpmb.com

[R56] 远程拷贝
来源：http://efm.tanke756.top

scp file user@host:/path/
来源：http://inu.jinqigufen.top

[R57] 远程执行命令
来源：http://nlz.epnwcf.com

ssh user@host 'uptime'
来源：http://kzr.quarkkingdee.top

[R58] 下载文件
来源：http://rmi.nanxuanxn.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://srm.cheryme.top

[R59] 发 POST JSON
来源：http://lop.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nzu.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://csn.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qze.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://xdx.jinghuilouyu.cn

df -h;  du -sh *
来源：http://lsn.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://hdj.jinqigufen.top

du -ah . | sort -rh | head -10
来源：http://jul.pycfn.com

[R63] 内存与进程
来源：http://xgl.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://suh.gogol.net.cn

[R64] 结束进程
来源：http://cxc.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://sdw.gaohongyu789.top

[R65] 查看端口占用
来源：http://rzb.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rxh.yvedp.cn

[R66] 定时任务
来源：http://uax.0kj1m.cn

crontab -e;  crontab -l
来源：http://gbq.cashguo.top

[R67] 生成随机十六进制串
来源：http://ndf.jqgufenzy.top

openssl rand -hex 16
来源：http://bmt.havefunace.top

[R68] 计算文件校验值
来源：http://bev.zhiwuduotai.top

sha256sum a.txt;  md5sum a.txt
来源：http://lhv.hcnkem.com

[R69] 生成随机密码
来源：http://slz.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://ffp.xziqi.cn

[R70] 时间戳与互转
来源：http://scx.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://xis.hammf.cn

[R71] 日期格式化
来源：http://nzz.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hus.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://ioz.gotoacloud.top

until nc -z localhost 3306; do sleep 1; done
来源：http://aqu.nanxuanxn.top

[R73] 分割大日志
来源：http://mvo.guowangkeji.top

split -l 1000 big.log part_
来源：http://dwb.xylfe.cn

[R74] 批量重命名
来源：http://qhw.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fqw.hysaishi.cn

[R75] 导出环境变量
来源：http://oqi.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://dmv.tanke756.top

[R76] 使用临时文件
来源：http://hwe.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ixh.yvedp.cn

[R77] 读取用户输入
来源：http://gby.zhengqikj.top


<!-- 参考信息 -->