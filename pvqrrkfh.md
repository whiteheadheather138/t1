代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gno.nwbrower.top

[Q26] 计数
来源：http://qli.kuanghao11.cn

SELECT COUNT(*) FROM users;
来源：http://nkn.epnwcf.com

[Q27] 条件计数
来源：http://gwf.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kfk.fzhhl.top

[Q28] 求和与平均
来源：http://kyh.pengpengdd.cyou

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mwf.yuanzhike.top

[Q29] 最大最小值
来源：http://vvl.daxiang520.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qzu.sysykeji.top

[Q30] 分组统计
来源：http://pua.yj202588.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ohc.cdnleiting.top

[Q31] 分组后过滤
来源：http://oyu.nanxuanxn.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xkm.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://ijf.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://edz.tanke756.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cfs.jyoumei.cn

[Q33] 多列分组
来源：http://gch.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xfh.pengpengdd.cyou

[Q34] 每组取第一条
来源：http://unz.mhx1999.top

SELECT * FROM (
来源：http://zhz.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ykh.gzhubu.top

) t WHERE rn = 1;
来源：http://uzo.sxryk.cn

[Q35] 内连接
来源：http://tyy.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ssd.zhoulong.xyz

[Q36] 左连接
来源：http://bfx.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cbm.sysykeji.top

[Q37] 右连接
来源：http://aoo.yanxiufei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://prl.tianlin.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://zwk.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ilm.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://hzt.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://piq.yfazqb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ond.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mbu.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fkb.vqdsnc.cn

[Q41] 多表连接
来源：http://vhs.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xdr.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://lng.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://gfn.jqgfzy.top

[Q42] 连接条件附加过滤
来源：http://lqs.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://edh.ywan-chungtsiang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ckc.ctjpmb.com

[Q43] 标量子查询
来源：http://leb.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://znp.gzhubu.top

[Q44] IN 子查询
来源：http://oua.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wnu.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://qhh.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://meh.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ihb.ivvv.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://keb.bjfxy.top

[Q47] 与平均值比较
来源：http://azg.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ivx.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://jcx.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mgk.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://tsc.aizwys.cn

[Q49] 更新单行
来源：http://pyq.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uka.zhengqikj.top

[Q50] 批量更新
来源：http://yzb.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tiv.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://eob.zhixingplan.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uvg.svipenyu.cn

[Q52] 删除指定行
来源：http://ipd.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://lmu.jyoumei.cn

[Q53] 按条件删除
来源：http://xbb.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vrb.guannengcc.top

[Q54] 清空表
来源：http://oxn.ivvv.top

TRUNCATE TABLE logs;
来源：http://emk.ybcxt.top

[Q55] 排名（并列占位）
来源：http://imt.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mca.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://wtk.zhiwuduotai.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://olk.yuxming.cn

[Q57] 行号
来源：http://dkv.hywenlv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://syu.nanxuanxn.top

[Q58] 累计求和
来源：http://xan.zhaomingkeji.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dfk.chenlongwang.top

[Q59] 分组内累计
来源：http://gvn.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://shn.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://qoy.jlsjyb.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ril.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uth.shuidangran.top

[Q61] 移动平均
来源：http://ruq.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://plu.fktsv.cn

[Q62] 分组占比
来源：http://hrw.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dso.shzxlz.cn

[Q63] 开启事务
来源：http://noz.wangdashe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bqz.vehdjk.com

[Q64] 提交事务
来源：http://gsf.daria6918.cn

COMMIT;
来源：http://bcq.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://ugg.shuidangran.top

ROLLBACK;
来源：http://zxv.yongpay.top

[Q66] 行锁查询
来源：http://dzl.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://any.hesvh.cn

[Q67] 设置隔离级别
来源：http://mzn.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fyy.52xcode.cn

[Q68] 保存点
来源：http://hmy.tanke756.top

SAVEPOINT sp1;
来源：http://lsg.haohaochexian.top

ROLLBACK TO sp1;
来源：http://auf.ppjwa.cn

[Q69] 查看执行计划
来源：http://teb.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://agp.ctjpmb.com

[Q70] 更新统计信息
来源：http://txc.vehdjk.com

ANALYZE TABLE users;
来源：http://dob.zdqjudy.top

[Q71] 查看建表语句
来源：http://hoi.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tew.jyoumei.cn

[Q72] 查看索引
来源：http://rlk.shuidangran.top

SHOW INDEX FROM users;
来源：http://jxb.nanxuanxn.top

[Q73] 查看表状态
来源：http://zov.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wcq.sweek.top

[Q74] 强制使用索引
来源：http://nab.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vsq.yuxming.cn

[Q75] 日期格式化
来源：http://phu.nanxinkj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gwz.shanyushiyangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dtb.uphjek.com

[Q76] 按天统计
来源：http://azl.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://txn.snrcjt.cn

[Q77] 时间加减
来源：http://ofa.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fae.tarul.cn

[Q78] 当前时间
来源：http://ary.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://med.dashuyun.cn

[Q79] 字符串拼接
来源：http://psh.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wgi.fehbvm.com

[Q80] 字符串截取
来源：http://auw.kuanghao11.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lbj.ctjpmb.com

[Q81] 字符串替换
来源：http://ufr.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zmk.shzxlz.cn

[Q82] 字符长度与字节长度
来源：http://aew.ppjwa.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fxg.xinyue.icu

[Q83] 大小写转换
来源：http://riy.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sla.316326.xyz

[Q84] 去除首尾空格
来源：http://ybq.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://zlx.shanyushiyangtech.top

[Q85] 数值取整
来源：http://aeq.tarul.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ysx.sufxvd.cn

[Q86] 读取 JSON 字段
来源：http://snm.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wtu.shuidangran.top

[Q87] JSON 字段做条件
来源：http://xht.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ikd.xingfuxueyuan.xyz

[Q88] 行转列（条件聚合）
来源：http://qhx.epnwcf.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rap.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sue.chenzaomai.com

[Q89] 判断表是否存在
来源：http://pcx.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cvb.jiagoushi.top

[Q90] 生成序号列
来源：http://kqi.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lit.jyoumei.cn

================================================================================
来源：http://twq.sysykeji.top

R. Bash 专题
来源：http://hxl.chenlongwang.top

================================================================================
来源：http://cws.0kj1m.cn

[R01] shebang 与严格模式
来源：http://ysb.sysykeji.top

#!/usr/bin/env bash
来源：http://uol.nanxuanxn.top

set -euo pipefail
来源：http://kxn.smart0.xyz

[R02] 变量赋值与使用
来源：http://xhc.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://sko.hysaishi.cn

[R03] 只读变量
来源：http://ewh.yueranfly.top

readonly PI=3.14
来源：http://cnk.yongpay.top

[R04] 位置参数
来源：http://dpb.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gol.jianghu66.top

[R05] 参数默认值
来源：http://lgz.iojbl.cn

name="${1:-default}"
来源：http://jbo.daria6918.cn

[R06] 判断命令是否存在
来源：http://mpw.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dns.pycfn.com

[R07] if 判断文件
来源：http://dah.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ysq.andypj.xyz

[R08] 数值比较
来源：http://cas.0kj1m.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wxp.pengpengdd.cyou

[R09] 字符串比较
来源：http://wgg.sxryk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://anj.xziqi.cn

[R10] 正则匹配
来源：http://eqh.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yzt.jyoumei.cn

[R11] case 多分支
来源：http://ucj.gotoacloud.top

case "$1" in
来源：http://paj.zdqjudy.top

start) echo "启动" ;;
来源：http://wsk.hcnkem.com

stop)  echo "停止" ;;
来源：http://mvh.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://jwo.hammf.cn

esac
来源：http://lpf.snrcjt.cn

[R12] for 遍历文件
来源：http://rzu.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://tgu.jqgfzy.top

[R13] for 计数循环
来源：http://sub.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://xdj.iojbl.cn

[R14] C 风格 for
来源：http://mxf.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kdf.snrcjt.cn

[R15] while 逐行读文件
来源：http://nmi.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wfy.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://piz.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kdp.xylfe.cn

[R17] 数组定义与取值
来源：http://aoh.sweek.top

arr=(a b c); echo "${arr[0]}"
来源：http://rxj.gogol.net.cn

[R18] 遍历数组
来源：http://wqx.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aka.cucudq.cn

[R19] 数组长度
来源：http://oyq.guannengcc.top

echo "${#arr[@]}"
来源：http://wrp.fengsongda.top

[R20] 关联数组（字典）
来源：http://msy.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qlg.nwbrower.top

[R21] 字符串长度
来源：http://ize.cheryme.top

echo "${#s}"
来源：http://ekx.meibo888.top

[R22] 截取子串
来源：http://vjj.havefunace.top

echo "${s:0:5}"
来源：http://tsn.aizwys.cn

[R23] 字符串替换
来源：http://kxu.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vki.jiagoushi.top

[R24] 大小写转换
来源：http://klv.jinqigufen.top

echo "${s^^}"; echo "${s,,}"
来源：http://esn.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://xvz.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qvy.jiagoushi.top

[R26] 命令替换
来源：http://rhm.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://zts.zhaomingkeji.xyz

[R27] 算术展开
来源：http://tan.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://txd.havefunace.top

[R28] 浮点运算
来源：http://fmw.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://qsk.guowangkeji.top

[R29] 定义函数
来源：http://isa.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oqc.yueranfly.top

[R30] 函数返回状态码
来源：http://rza.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://nyw.jiagoushi.top

[R31] 局部变量
来源：http://dgz.jinqigufen.top

f() { local x=1; echo "$x"; }
来源：http://uee.sufxvd.cn

[R32] 参数个数校验
来源：http://lgi.fengsongda.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hya.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://vhn.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jyi.jiagoushi.top

[R34] 退出时清理
来源：http://oih.ctjpmb.com

trap 'rm -f "$tmp"' EXIT
来源：http://tsa.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://wci.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://aht.haohaochexian.top

[R36] 并发执行多个任务
来源：http://tjo.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lra.ywan-chungtsiang.top

[R37] 把输出赋给变量
来源：http://rqe.chenzaomai.com

files=$(ls -1)
来源：http://etr.sweek.top

[R38] 管道串联
来源：http://cqv.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://fzh.havefunace.top

[R39] 重定向标准输出与错误
来源：http://hur.daxiang520.top

cmd > out.log 2>&1
来源：http://xgi.sweek.top

[R40] 追加写日志
来源：http://xuw.yj202588.top

echo "log" >> out.log
来源：http://lpd.shangyingyoupin.top

[R41] 丢弃输出
来源：http://mia.sjlbkw.cn

cmd >/dev/null 2>&1
来源：http://izw.yuxming.cn

[R42] 输入重定向
来源：http://sxb.nanxinkj.top

wc -l < a.txt
来源：http://lci.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://wlg.sweek.top

find . -name "*.log" -type f
来源：http://pmi.yueranfly.top

[R44] 按修改时间查找
来源：http://pmf.daxiang520.top

find . -mtime -7 -type f
来源：http://nuu.hammf.cn

[R45] 批量删除
来源：http://ofw.fehbvm.com

find . -name "*.tmp" -delete
来源：http://feh.ehwqpu.com

[R46] 递归替换文件内容
来源：http://xfg.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xjn.yangfankeji.com

[R47] sed 单行替换
来源：http://bmp.9152youxi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hkv.gogol.net.cn

[R48] awk 取指定列
来源：http://urv.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://piw.c1oappe.top

[R49] awk 带条件
来源：http://udv.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tgo.ydjk.org.cn

[R50] awk 求和
来源：http://uqj.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://rfk.vqdsnc.cn

[R51] 排序去重取前几
来源：http://zwe.pengpengdd.cyou

sort a.txt | uniq -c | sort -rn | head
来源：http://qju.sxryk.cn

[R52] 统计行数
来源：http://fpz.yfazqb.com

wc -l a.txt
来源：http://hdk.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://ggc.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gfg.haohaochexian.top

[R54] 比较两个文件
来源：http://jry.yuxming.cn

diff a.txt b.txt
来源：http://odv.nanxinkj.top

[R55] 压缩与解压
来源：http://xvv.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pjx.vehdjk.com

[R56] 远程拷贝
来源：http://fwi.cashguo.top

scp file user@host:/path/
来源：http://uzv.sjlbkw.cn

[R57] 远程执行命令
来源：http://mzd.52xcode.cn

ssh user@host 'uptime'
来源：http://dgh.zhaomingkeji.xyz

[R58] 下载文件
来源：http://jav.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wvw.hywenlv.cn

[R59] 发 POST JSON
来源：http://gzz.bbcook.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jig.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://kld.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fkz.chenlongwang.top

[R61] 磁盘占用
来源：http://jew.ctjpmb.com

df -h;  du -sh *
来源：http://pud.ehwqpu.com

[R62] 找最占空间的文件
来源：http://ioh.jinqigufen.top

du -ah . | sort -rh | head -10
来源：http://git.ehwqpu.com

[R63] 内存与进程
来源：http://vat.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://wat.yangfankeji.com

[R64] 结束进程
来源：http://zkw.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://djr.dianchejie.cn

[R65] 查看端口占用
来源：http://cex.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zpg.zdbjq.cn

[R66] 定时任务
来源：http://sir.yj20258888.top

crontab -e;  crontab -l
来源：http://bzg.guannengcc.top

[R67] 生成随机十六进制串
来源：http://coz.xinyue.icu

openssl rand -hex 16
来源：http://pla.sysykeji.top

[R68] 计算文件校验值
来源：http://ljl.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ubx.cucudq.cn

[R69] 生成随机密码
来源：http://vud.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://iot.tanke756.top

[R70] 时间戳与互转
来源：http://sma.bbcook.cn

date +%s;  date -d @1700000000
来源：http://npj.guannengcc.top

[R71] 日期格式化
来源：http://eeo.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jwl.xinyue.icu

[R72] 等待端口就绪
来源：http://vaw.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yfm.zycfv.cn

[R73] 分割大日志
来源：http://hxi.vqdsnc.cn

split -l 1000 big.log part_
来源：http://tmf.feifeiyinyue.top

[R74] 批量重命名
来源：http://vry.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bjp.ydzc1.top

[R75] 导出环境变量
来源：http://nrd.shzxlz.cn


<!-- 参考信息 -->