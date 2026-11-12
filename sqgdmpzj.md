代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://avc.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://bxl.pycfn.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sar.sysykeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ljf.hysaishi.cn

[Q33] 多列分组
来源：http://vgt.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rjp.tianlin.xyz

[Q34] 每组取第一条
来源：http://lne.yfazqb.com

SELECT * FROM (
来源：http://ane.yuanzhike.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bku.chenzaomai.com

) t WHERE rn = 1;
来源：http://aoy.dianchejie.cn

[Q35] 内连接
来源：http://pnh.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fro.cqqwz.cn

[Q36] 左连接
来源：http://nmv.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qxz.shangyingyoupin.top

[Q37] 右连接
来源：http://ftt.ivvv.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ygt.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://cng.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xzc.kuanghao11.cn

[Q39] 自连接（查上下级）
来源：http://uvi.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hvv.nwbrower.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qrc.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://apt.ppjwa.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xxh.zhijiandao.cn

[Q41] 多表连接
来源：http://jic.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sdy.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://chh.jinqigufen.top

JOIN products p ON p.id = o.product_id;
来源：http://dps.yonumen.top

[Q42] 连接条件附加过滤
来源：http://icy.fktsv.cn

SELECT u.name, o.amount FROM users u
来源：http://ycx.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zbh.wangdashe.top

[Q43] 标量子查询
来源：http://abb.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://udt.fengsongda.top

[Q44] IN 子查询
来源：http://ica.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ifj.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://bpu.zhixingplan.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xny.ydjk.org.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ipt.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ohj.zhixingplan.top

[Q47] 与平均值比较
来源：http://ywj.jinqigfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rfz.guowangkeji.top

[Q48] CTE 公用表表达式
来源：http://iai.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bzt.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://hul.gogol.net.cn

[Q49] 更新单行
来源：http://asy.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nab.zdbjq.cn

[Q50] 批量更新
来源：http://hvb.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aga.vqdsnc.cn

[Q51] 用子查询更新
来源：http://rgj.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sre.zhixingplan.top

[Q52] 删除指定行
来源：http://kcu.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://rpu.guowangkeji.top

[Q53] 按条件删除
来源：http://eli.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nae.fengsongda.top

[Q54] 清空表
来源：http://iww.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://hub.jinqigfzy.top

[Q55] 排名（并列占位）
来源：http://gdg.tianlin.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sol.yangfankeji.com

[Q56] 密集排名（并列不占位）
来源：http://scg.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yaj.nanxuanxn.top

[Q57] 行号
来源：http://biq.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zzv.jqgfzy.top

[Q58] 累计求和
来源：http://qha.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wuq.zycfv.cn

[Q59] 分组内累计
来源：http://uil.shangyingyoupin.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fuq.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://vrt.tian-w.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ntz.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ksv.bbcook.cn

[Q61] 移动平均
来源：http://mmh.andypj.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rcc.yueranfly.top

[Q62] 分组占比
来源：http://eko.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ebo.cqqwz.cn

[Q63] 开启事务
来源：http://iue.tanke756.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bzj.svipenyu.cn

[Q64] 提交事务
来源：http://vzi.hysaishi.cn

COMMIT;
来源：http://nyw.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://wqj.ywan-chungtsiang.top

ROLLBACK;
来源：http://egi.xuanzx.com

[Q66] 行锁查询
来源：http://lrm.gzhubu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xjn.fengsongda.top

[Q67] 设置隔离级别
来源：http://vvh.daxiang520.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qlx.vqdsnc.cn

[Q68] 保存点
来源：http://yvl.pycfn.com

SAVEPOINT sp1;
来源：http://stu.chenlongwang.top

ROLLBACK TO sp1;
来源：http://zpg.fktsv.cn

[Q69] 查看执行计划
来源：http://atl.xingfuxueyuan.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tjt.sysykeji.top

[Q70] 更新统计信息
来源：http://fho.aibaodan.cn

ANALYZE TABLE users;
来源：http://jix.bbcook.cn

[Q71] 查看建表语句
来源：http://zcv.fehbvm.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kfy.iojbl.cn

[Q72] 查看索引
来源：http://aqa.tarul.cn

SHOW INDEX FROM users;
来源：http://xlk.hywenlv.cn

[Q73] 查看表状态
来源：http://pql.jinqigfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ker.sysykeji.top

[Q74] 强制使用索引
来源：http://avw.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ngm.zhoulong.xyz

[Q75] 日期格式化
来源：http://mee.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://flb.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pwx.dashuyun.cn

[Q76] 按天统计
来源：http://gqv.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rwe.316326.xyz

[Q77] 时间加减
来源：http://xsj.tarul.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tdj.sufxvd.cn

[Q78] 当前时间
来源：http://nen.sweek.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://osb.zhoulong.xyz

[Q79] 字符串拼接
来源：http://vop.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wnp.fehbvm.com

[Q80] 字符串截取
来源：http://yqt.fanxiaobao.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://que.jinqigufen.top

[Q81] 字符串替换
来源：http://pgi.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iuo.yj20258888.top

[Q82] 字符长度与字节长度
来源：http://zlv.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aib.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://lxz.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://grl.pycfn.com

[Q84] 去除首尾空格
来源：http://kgx.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://qba.wangshuangyany.cn

[Q85] 数值取整
来源：http://snl.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yps.gogol.net.cn

[Q86] 读取 JSON 字段
来源：http://odq.zdbjq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xsn.yuxming.cn

[Q87] JSON 字段做条件
来源：http://don.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://irs.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://qeu.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cnc.zdqjudy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zma.pycfn.com

[Q89] 判断表是否存在
来源：http://fzd.gotoacloud.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hnt.ydzc1.top

[Q90] 生成序号列
来源：http://yci.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dym.hongshengwenyu.top

================================================================================
来源：http://bsp.fzhhl.top

R. Bash 专题
来源：http://eun.zhengqikj.top

================================================================================
来源：http://cva.c1oappe.top

[R01] shebang 与严格模式
来源：http://kcl.0kj1m.cn

#!/usr/bin/env bash
来源：http://hsj.nanxinkj.top

set -euo pipefail
来源：http://jze.fktsv.cn

[R02] 变量赋值与使用
来源：http://ofo.ppjwa.cn

name="Tom"; echo "$name"
来源：http://rwr.pengpengdd.cyou

[R03] 只读变量
来源：http://iwp.cheryme.top

readonly PI=3.14
来源：http://twj.yuanzhike.top

[R04] 位置参数
来源：http://kcq.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ohv.bbcook.cn

[R05] 参数默认值
来源：http://xrk.pengpengdd.cyou

name="${1:-default}"
来源：http://lps.fktsv.cn

[R06] 判断命令是否存在
来源：http://ebo.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fus.hongshengwenyu.top

[R07] if 判断文件
来源：http://xjq.zdqjudy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kxv.birdmap.top

[R08] 数值比较
来源：http://alf.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xbk.tian-w.cn

[R09] 字符串比较
来源：http://sqw.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dxu.kuanghao11.cn

[R10] 正则匹配
来源：http://uxp.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ysk.cheryme.top

[R11] case 多分支
来源：http://lhk.xinyue.icu

case "$1" in
来源：http://zcu.andypj.xyz

start) echo "启动" ;;
来源：http://tkw.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://ldn.yfazqb.com

*)     echo "未知命令" ;;
来源：http://dwg.sysykeji.top

esac
来源：http://ipm.hammf.cn

[R12] for 遍历文件
来源：http://kqy.ehwqpu.com

for f in *.txt; do echo "$f"; done
来源：http://lyw.fengsongda.top

[R13] for 计数循环
来源：http://ofk.52xcode.cn

for i in {1..10}; do echo "$i"; done
来源：http://mff.vqdsnc.cn

[R14] C 风格 for
来源：http://mqb.birdmap.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bat.bbcook.cn

[R15] while 逐行读文件
来源：http://knz.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://trm.fzhhl.top

[R16] until 等待条件
来源：http://dee.pycfn.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dgs.xylfe.cn

[R17] 数组定义与取值
来源：http://ywf.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://zhy.xinyue.icu

[R18] 遍历数组
来源：http://jqu.hywenlv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ewr.andypj.xyz

[R19] 数组长度
来源：http://zwo.zycfv.cn

echo "${#arr[@]}"
来源：http://klk.gzhubu.top

[R20] 关联数组（字典）
来源：http://mpn.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bfx.haohaochexian.top

[R21] 字符串长度
来源：http://hpz.fktsv.cn

echo "${#s}"
来源：http://zjy.ppjwa.cn

[R22] 截取子串
来源：http://flt.ctjpmb.com

echo "${s:0:5}"
来源：http://siv.nanxuanxn.top

[R23] 字符串替换
来源：http://uvq.sjlbkw.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fkx.ydzc1.top

[R24] 大小写转换
来源：http://gek.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://ynv.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://nbk.wangdashe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://psh.tanke756.top

[R26] 命令替换
来源：http://bbt.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://pim.jianghu66.top

[R27] 算术展开
来源：http://taz.yfazqb.com

echo $((1 + 2 * 3))
来源：http://mxw.zhongyouzk.top

[R28] 浮点运算
来源：http://wen.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://lat.meibo888.top

[R29] 定义函数
来源：http://kjf.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tra.yueranfly.top

[R30] 函数返回状态码
来源：http://tdn.xuanzx.com

f() { return 0; }; f || echo "失败了"
来源：http://mql.hysaishi.cn

[R31] 局部变量
来源：http://lvl.haohaochexian.top

f() { local x=1; echo "$x"; }
来源：http://gzg.sufxvd.cn

[R32] 参数个数校验
来源：http://fav.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zhg.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://eea.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qqa.tarul.cn

[R34] 退出时清理
来源：http://snp.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://qaq.jinqigufen.top

[R35] 后台执行并等待
来源：http://shn.yj20258888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://czr.gzhubu.top

[R36] 并发执行多个任务
来源：http://nuc.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hpv.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://sgu.gogol.net.cn

files=$(ls -1)
来源：http://cia.gzhubu.top

[R38] 管道串联
来源：http://rrm.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://mif.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://ywv.zhixingplan.top

cmd > out.log 2>&1
来源：http://hqc.yfazqb.com

[R40] 追加写日志
来源：http://alz.fktsv.cn

echo "log" >> out.log
来源：http://vhy.bjfxy.top

[R41] 丢弃输出
来源：http://prf.xylfe.cn

cmd >/dev/null 2>&1
来源：http://zdw.sjlbkw.cn

[R42] 输入重定向
来源：http://hfh.tanke756.top

wc -l < a.txt
来源：http://hcw.fengsongda.top

[R43] 按名字查找文件
来源：http://pvm.iojbl.cn

find . -name "*.log" -type f
来源：http://mza.9152youxi.cn

[R44] 按修改时间查找
来源：http://rpv.chenlongwang.top

find . -mtime -7 -type f
来源：http://gmi.pengpengdd.cyou

[R45] 批量删除
来源：http://wuu.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://nth.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://njx.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fww.vqdsnc.cn

[R47] sed 单行替换
来源：http://hca.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iko.jinqigufen.top

[R48] awk 取指定列
来源：http://kpl.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://jno.tianlin.xyz

[R49] awk 带条件
来源：http://lia.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://npj.gzhubu.top

[R50] awk 求和
来源：http://dwx.hfpthk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vjf.cqqwz.cn

[R51] 排序去重取前几
来源：http://uys.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://itn.vqdsnc.cn

[R52] 统计行数
来源：http://kbf.gotoacloud.top

wc -l a.txt
来源：http://icl.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://rcd.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zfo.hammf.cn

[R54] 比较两个文件
来源：http://wdn.jinghuilouyu.cn

diff a.txt b.txt
来源：http://zfe.316326.xyz

[R55] 压缩与解压
来源：http://yhq.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uus.hcnkem.com

[R56] 远程拷贝
来源：http://sri.xinyue.icu

scp file user@host:/path/
来源：http://hbp.kuanghao11.cn

[R57] 远程执行命令
来源：http://kch.jinqigufen.top

ssh user@host 'uptime'
来源：http://ctr.gogol.net.cn

[R58] 下载文件
来源：http://slx.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://poj.dashuyun.cn

[R59] 发 POST JSON
来源：http://hif.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ope.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://bte.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gbm.cashguo.top

[R61] 磁盘占用
来源：http://jgg.dashuyun.cn

df -h;  du -sh *
来源：http://pqn.dianchejie.cn

[R62] 找最占空间的文件
来源：http://gso.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://keh.shuidangran.top

[R63] 内存与进程
来源：http://hoj.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://xws.xylfe.cn

[R64] 结束进程
来源：http://bbm.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://ylr.zhongyouzk.top

[R65] 查看端口占用
来源：http://fje.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ilg.dashuyun.cn

[R66] 定时任务
来源：http://wgv.shuidangran.top

crontab -e;  crontab -l
来源：http://nkq.pycfn.com

[R67] 生成随机十六进制串
来源：http://vux.ywan-chungtsiang.top

openssl rand -hex 16
来源：http://onl.zdqjudy.top

[R68] 计算文件校验值
来源：http://lgg.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pbl.xuanzx.com

[R69] 生成随机密码
来源：http://nxq.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://kzh.dianchejie.cn

[R70] 时间戳与互转
来源：http://wvy.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://qzf.xingfuxueyuan.xyz

[R71] 日期格式化
来源：http://qpr.sweek.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xli.ydzc1.top

[R72] 等待端口就绪
来源：http://jvn.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qqc.316326.xyz

[R73] 分割大日志
来源：http://ois.sysykeji.top

split -l 1000 big.log part_
来源：http://olz.yangfankeji.com

[R74] 批量重命名
来源：http://rma.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nib.bjfxy.top

[R75] 导出环境变量
来源：http://fli.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://uee.316326.xyz

[R76] 使用临时文件
来源：http://dei.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dzd.redwolf501.top

[R77] 读取用户输入
来源：http://qsl.aibaodan.cn

read -rp "请输入: " ans
来源：http://kik.cqqwz.cn

[R78] 交互式菜单
来源：http://hpr.pycfn.com

select opt in a b c; do echo "$opt"; break; done
来源：http://cvj.birdmap.top

[R79] 解析命令行选项
来源：http://eys.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lqq.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://cdx.cucudq.cn

time ./run.sh
来源：http://kip.hfpthk.cn

================================================================================
来源：http://mdc.quarkkingdee.top


<!-- 参考信息 -->