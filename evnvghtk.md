代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://njb.hammf.cn

[Q32] 分组拼接字符串
来源：http://chg.52xcode.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jcs.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xjm.c1oappe.top

[Q33] 多列分组
来源：http://mwj.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://toz.dashuyun.cn

[Q34] 每组取第一条
来源：http://xng.52xcode.cn

SELECT * FROM (
来源：http://dwt.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ypt.dianchejie.cn

) t WHERE rn = 1;
来源：http://ewa.hesvh.cn

[Q35] 内连接
来源：http://buj.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://awl.shuidangran.top

[Q36] 左连接
来源：http://evz.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hgd.shangyingyoupin.top

[Q37] 右连接
来源：http://rze.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yyn.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://zeu.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://flr.wangshuangyany.cn

[Q39] 自连接（查上下级）
来源：http://ttz.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mgv.havefunace.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jaa.birdmap.top

[Q40] 交叉连接（笛卡尔积）
来源：http://doi.vqdsnc.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aju.fehbvm.com

[Q41] 多表连接
来源：http://qaf.ctjpmb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://fuu.zycfv.cn

JOIN users u ON u.id = o.user_id
来源：http://qdn.hysaishi.cn

JOIN products p ON p.id = o.product_id;
来源：http://psz.52xcode.cn

[Q42] 连接条件附加过滤
来源：http://gzl.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://kxi.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://azy.yj20258888.top

[Q43] 标量子查询
来源：http://dwj.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gjp.bjfxy.top

[Q44] IN 子查询
来源：http://gyf.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://auy.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://fpt.yueranfly.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mjm.zhixingplan.top

[Q46] NOT EXISTS 判断不存在
来源：http://pip.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zlf.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://nqa.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dil.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://wsy.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yiu.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://rfd.guowangkeji.top

[Q49] 更新单行
来源：http://krb.xuanzx.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yny.zycfv.cn

[Q50] 批量更新
来源：http://ruk.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tyh.ydjk.org.cn

[Q51] 用子查询更新
来源：http://izb.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://otw.jinqigfzy.top

[Q52] 删除指定行
来源：http://zck.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://upp.9152youxi.cn

[Q53] 按条件删除
来源：http://htj.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qfg.cucudq.cn

[Q54] 清空表
来源：http://rnw.smart0.xyz

TRUNCATE TABLE logs;
来源：http://ztl.fehbvm.com

[Q55] 排名（并列占位）
来源：http://zrn.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://msn.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://euu.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hoi.cashguo.top

[Q57] 行号
来源：http://vgs.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rfy.sjlbkw.cn

[Q58] 累计求和
来源：http://onb.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vlq.dianchejie.cn

[Q59] 分组内累计
来源：http://fbf.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gvy.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://pmp.zycfv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iyd.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nkt.guowangkeji.top

[Q61] 移动平均
来源：http://ojo.havefunace.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jvq.shanyushiyangkeji.top

[Q62] 分组占比
来源：http://ocn.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://phr.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://nfv.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rhs.tarul.cn

[Q64] 提交事务
来源：http://uxp.epnwcf.com

COMMIT;
来源：http://qtd.dianchejie.cn

[Q65] 回滚事务
来源：http://vki.nanxuanxn.top

ROLLBACK;
来源：http://zer.zhongyouzk.top

[Q66] 行锁查询
来源：http://efa.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nlg.xingfuxueyuan.xyz

[Q67] 设置隔离级别
来源：http://lse.yj202588.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qrn.jianghu66.top

[Q68] 保存点
来源：http://byb.jqgufenzy.top

SAVEPOINT sp1;
来源：http://dmq.yfazqb.com

ROLLBACK TO sp1;
来源：http://mas.ybcxt.top

[Q69] 查看执行计划
来源：http://vqi.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lvc.jqgufenzy.top

[Q70] 更新统计信息
来源：http://gmy.zhoulong.xyz

ANALYZE TABLE users;
来源：http://wjj.cashguo.top

[Q71] 查看建表语句
来源：http://yvk.jqgufenzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://czz.hnqzz.top

[Q72] 查看索引
来源：http://mlf.guowangkeji.top

SHOW INDEX FROM users;
来源：http://ccm.zhiwuduotai.top

[Q73] 查看表状态
来源：http://hvw.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ave.ydzc1.top

[Q74] 强制使用索引
来源：http://fxd.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jae.aizwys.cn

[Q75] 日期格式化
来源：http://eip.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aln.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ofl.zhijiandao.cn

[Q76] 按天统计
来源：http://yyv.vqdsnc.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ihz.316326.xyz

[Q77] 时间加减
来源：http://zit.xingfuxueyuan.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://slj.xinyue.icu

[Q78] 当前时间
来源：http://wes.yuanzhike.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hxi.epnwcf.com

[Q79] 字符串拼接
来源：http://vij.ctjpmb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hol.jyoumei.cn

[Q80] 字符串截取
来源：http://biz.bbcook.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gxt.gogol.net.cn

[Q81] 字符串替换
来源：http://hpo.fzhhl.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nrp.nanxuanxn.top

[Q82] 字符长度与字节长度
来源：http://sne.yuanzhike.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hbp.0kj1m.cn

[Q83] 大小写转换
来源：http://tji.smart0.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://clt.jinqigufen.top

[Q84] 去除首尾空格
来源：http://rnn.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://rhs.guowangkeji.top

[Q85] 数值取整
来源：http://zbu.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://guq.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://yex.pengpengdd.cyou

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jca.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://pcv.shanyushiyangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ifa.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://ytu.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gbe.zdqjudy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nmh.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://ctw.xuetiantiany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uyl.hongshengwenyu.top

[Q90] 生成序号列
来源：http://cqh.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xtc.havefunace.top

================================================================================
来源：http://iyz.quarkkingdee.top

R. Bash 专题
来源：http://mxy.yongpay.top

================================================================================
来源：http://kos.nwbrower.top

[R01] shebang 与严格模式
来源：http://hbm.andypj.xyz

#!/usr/bin/env bash
来源：http://bga.jqgfzy.top

set -euo pipefail
来源：http://ziv.jiagoushi.top

[R02] 变量赋值与使用
来源：http://iox.ehwqpu.com

name="Tom"; echo "$name"
来源：http://ovw.sysykeji.top

[R03] 只读变量
来源：http://asi.guowangkeji.top

readonly PI=3.14
来源：http://hoi.jqgfzy.top

[R04] 位置参数
来源：http://ixp.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://swk.ppjwa.cn

[R05] 参数默认值
来源：http://rse.redwolf501.top

name="${1:-default}"
来源：http://vdc.zycfv.cn

[R06] 判断命令是否存在
来源：http://gwv.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qgz.nanxuanxn.top

[R07] if 判断文件
来源：http://dwa.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ivd.hfpthk.cn

[R08] 数值比较
来源：http://kob.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sxp.chenzaomai.com

[R09] 字符串比较
来源：http://elm.shanyushiyangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jma.mhx1999.top

[R10] 正则匹配
来源：http://dkx.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://shn.fktsv.cn

[R11] case 多分支
来源：http://iob.zhiwuduotai.top

case "$1" in
来源：http://iww.redwolf501.top

start) echo "启动" ;;
来源：http://nhw.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://fsy.tian-w.cn

*)     echo "未知命令" ;;
来源：http://lbj.jlsjyb.cn

esac
来源：http://shn.yj20258.top

[R12] for 遍历文件
来源：http://qhd.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://sxx.hfpthk.cn

[R13] for 计数循环
来源：http://jmb.gzhubu.top

for i in {1..10}; do echo "$i"; done
来源：http://qrq.pycfn.com

[R14] C 风格 for
来源：http://xdq.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://syz.sufxvd.cn

[R15] while 逐行读文件
来源：http://ljr.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lca.smart0.xyz

[R16] until 等待条件
来源：http://unw.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jax.svipenyu.cn

[R17] 数组定义与取值
来源：http://xqc.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jmr.fktsv.cn

[R18] 遍历数组
来源：http://lsg.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://szc.ehwqpu.com

[R19] 数组长度
来源：http://hch.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://dsn.daria6918.cn

[R20] 关联数组（字典）
来源：http://efo.tarul.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://klb.hesvh.cn

[R21] 字符串长度
来源：http://emj.zhoulong.xyz

echo "${#s}"
来源：http://xbf.fanxiaobao.xyz

[R22] 截取子串
来源：http://vum.cashguo.top

echo "${s:0:5}"
来源：http://iqc.zhixingplan.top

[R23] 字符串替换
来源：http://cvz.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://imh.zhoulong.xyz

[R24] 大小写转换
来源：http://dfp.0kj1m.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pib.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://tjs.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bgz.gogol.net.cn

[R26] 命令替换
来源：http://evc.yvedp.cn

now=$(date +%F); echo "$now"
来源：http://pfb.xylfe.cn

[R27] 算术展开
来源：http://zpx.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://jxr.cashguo.top

[R28] 浮点运算
来源：http://kof.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://nxy.0kj1m.cn

[R29] 定义函数
来源：http://veh.zhoulong.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rvi.hywenlv.cn

[R30] 函数返回状态码
来源：http://xca.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://jrw.guannengcc.top

[R31] 局部变量
来源：http://sdy.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://pll.9152youxi.cn

[R32] 参数个数校验
来源：http://rcl.tarul.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wck.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://qih.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jxw.vqdsnc.cn

[R34] 退出时清理
来源：http://zde.yongpay.top

trap 'rm -f "$tmp"' EXIT
来源：http://zez.iojbl.cn

[R35] 后台执行并等待
来源：http://tfr.quarkkingdee.top

sleep 5 & pid=$!; wait "$pid"
来源：http://eab.snrcjt.cn

[R36] 并发执行多个任务
来源：http://ltn.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://loh.ctjpmb.com

[R37] 把输出赋给变量
来源：http://kzl.zhengqikj.top

files=$(ls -1)
来源：http://qog.yangfankeji.com

[R38] 管道串联
来源：http://lyw.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://brt.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://jzk.uphjek.com

cmd > out.log 2>&1
来源：http://lpv.316326.xyz

[R40] 追加写日志
来源：http://qqu.fzhhl.top

echo "log" >> out.log
来源：http://wdu.ydjk.org.cn

[R41] 丢弃输出
来源：http://ppt.jyoumei.cn

cmd >/dev/null 2>&1
来源：http://bla.redwolf501.top

[R42] 输入重定向
来源：http://gzs.c1oappe.top

wc -l < a.txt
来源：http://lja.ydzc1.top

[R43] 按名字查找文件
来源：http://iuu.guowangkeji.top

find . -name "*.log" -type f
来源：http://fvb.vqdsnc.cn

[R44] 按修改时间查找
来源：http://gva.0kj1m.cn

find . -mtime -7 -type f
来源：http://drd.nanxinkj.top

[R45] 批量删除
来源：http://rkj.yuxming.cn

find . -name "*.tmp" -delete
来源：http://xqd.svipenyu.cn

[R46] 递归替换文件内容
来源：http://nwo.yj20258.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zvk.ppjwa.cn

[R47] sed 单行替换
来源：http://sck.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://jsv.zdbjq.cn

[R48] awk 取指定列
来源：http://sgp.pengpengdd.cyou

awk '{print $1, $3}' a.txt
来源：http://jst.hcnkem.com

[R49] awk 带条件
来源：http://jkg.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ywr.shzxlz.cn

[R50] awk 求和
来源：http://dfl.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kfj.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://mjh.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hjk.nanxuanxn.top

[R52] 统计行数
来源：http://oia.nanxuanxn.top

wc -l a.txt
来源：http://wme.cashguo.top

[R53] 查看文件头与实时尾
来源：http://vcd.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dyv.kuanghao11.cn

[R54] 比较两个文件
来源：http://kwx.hcnkem.com

diff a.txt b.txt
来源：http://bsr.snrcjt.cn

[R55] 压缩与解压
来源：http://hjz.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nuw.fktsv.cn

[R56] 远程拷贝
来源：http://vdq.yfazqb.com

scp file user@host:/path/
来源：http://cmb.jyoumei.cn

[R57] 远程执行命令
来源：http://adm.ehwqpu.com

ssh user@host 'uptime'
来源：http://qsh.shanyushiyangkeji.top

[R58] 下载文件
来源：http://btc.yonumen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jgo.hfpthk.cn

[R59] 发 POST JSON
来源：http://ymy.bbcook.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pbz.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://eks.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://atb.ivvv.top

[R61] 磁盘占用
来源：http://ryo.smart0.xyz

df -h;  du -sh *
来源：http://ocz.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://sng.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://qln.hywenlv.cn

[R63] 内存与进程
来源：http://pxo.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://aly.redwolf501.top

[R64] 结束进程
来源：http://gpj.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://soi.gogol.net.cn

[R65] 查看端口占用
来源：http://jly.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://otl.xziqi.cn

[R66] 定时任务
来源：http://axo.aibaodan.cn

crontab -e;  crontab -l
来源：http://jud.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://hyv.jinqigufen.top

openssl rand -hex 16
来源：http://jhg.52xcode.cn

[R68] 计算文件校验值
来源：http://wik.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://lax.fktsv.cn

[R69] 生成随机密码
来源：http://fdz.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://vcp.zhixingplan.top

[R70] 时间戳与互转
来源：http://jvv.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://ira.yj202588.top

[R71] 日期格式化
来源：http://mfa.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hxc.jiagoushi.top

[R72] 等待端口就绪
来源：http://kop.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://jll.wangdashe.top

[R73] 分割大日志
来源：http://bua.shangyingyoupin.top

split -l 1000 big.log part_
来源：http://lfo.xinyue.icu

[R74] 批量重命名
来源：http://kiz.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mft.yanxiufei.cn

[R75] 导出环境变量
来源：http://ura.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://ehl.shangyingyoupin.top

[R76] 使用临时文件
来源：http://qpj.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wcw.yj20258888.top

[R77] 读取用户输入
来源：http://jqk.xuetiantiany.cn

read -rp "请输入: " ans
来源：http://zgm.sweek.top

[R78] 交互式菜单
来源：http://fzw.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://taf.chenzaomai.com

[R79] 解析命令行选项
来源：http://mvh.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yir.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://ehx.andypj.xyz

time ./run.sh
来源：http://ysn.pycfn.com

================================================================================
来源：http://fye.jqgfzy.top


<!-- 参考信息 -->