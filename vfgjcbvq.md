代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bwe.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://bng.cqqwz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tdz.yonumen.top

[Q29] 最大最小值
来源：http://pet.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pkl.ctjpmb.com

[Q30] 分组统计
来源：http://etk.jinqigufen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gyq.yvedp.cn

[Q31] 分组后过滤
来源：http://kpx.vqdsnc.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dhh.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://swy.gotoacloud.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xhx.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hew.ydzc1.top

[Q33] 多列分组
来源：http://gdh.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tzb.bjfxy.top

[Q34] 每组取第一条
来源：http://rab.ywan-chungtsiang.top

SELECT * FROM (
来源：http://nfs.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://guv.yuanzhike.top

) t WHERE rn = 1;
来源：http://tdg.ydzc1.top

[Q35] 内连接
来源：http://wsh.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aov.jinyuanbaomall.cn

[Q36] 左连接
来源：http://zyi.guannengcc.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ydb.ivvv.top

[Q37] 右连接
来源：http://xbk.chenlongwang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pfz.uphjek.com

[Q38] 全外连接（PostgreSQL）
来源：http://vzq.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vgr.fanxiaobao.xyz

[Q39] 自连接（查上下级）
来源：http://fqv.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tco.c1oappe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lcc.tian-w.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xbe.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rdl.hcnkem.com

[Q41] 多表连接
来源：http://whe.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bnm.cheryme.top

JOIN users u ON u.id = o.user_id
来源：http://jpr.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://abw.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://bim.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://bim.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pfb.uphjek.com

[Q43] 标量子查询
来源：http://sld.zhixingplan.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zgh.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://czl.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yke.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://byn.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kwf.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://ejf.tian-w.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qbs.zhoulong.xyz

[Q47] 与平均值比较
来源：http://oag.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pmv.mhx1999.top

[Q48] CTE 公用表表达式
来源：http://jpu.zhixingplan.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sbn.gaohongyu789.top

SELECT * FROM t WHERE c > 5;
来源：http://bta.smart0.xyz

[Q49] 更新单行
来源：http://jeg.aizwys.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qca.daxiang520.top

[Q50] 批量更新
来源：http://mry.meibo888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wou.kuanghao11.cn

[Q51] 用子查询更新
来源：http://xyb.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rli.hnxiangtu.top

[Q52] 删除指定行
来源：http://tyy.smart0.xyz

DELETE FROM users WHERE id = 10;
来源：http://uyl.haohaochexian.top

[Q53] 按条件删除
来源：http://vgr.zhoulong.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hdj.hammf.cn

[Q54] 清空表
来源：http://ith.ydzc1.top

TRUNCATE TABLE logs;
来源：http://ofa.yongpay.top

[Q55] 排名（并列占位）
来源：http://fzh.sxryk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eym.nwbrower.top

[Q56] 密集排名（并列不占位）
来源：http://led.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aik.yongpay.top

[Q57] 行号
来源：http://chw.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ets.yj20258888.top

[Q58] 累计求和
来源：http://fru.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aon.daxiang520.top

[Q59] 分组内累计
来源：http://dqi.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jel.ehwqpu.com

[Q60] 取上一行 / 下一行
来源：http://dse.hcnkem.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gwg.jyoumei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nlf.zycfv.cn

[Q61] 移动平均
来源：http://bwn.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wgt.fktsv.cn

[Q62] 分组占比
来源：http://vnk.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://klx.fzhhl.top

[Q63] 开启事务
来源：http://bhg.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://hkx.c1oappe.top

[Q64] 提交事务
来源：http://eln.vehdjk.com

COMMIT;
来源：http://nwj.aizwys.cn

[Q65] 回滚事务
来源：http://puc.iojbl.cn

ROLLBACK;
来源：http://gtr.hnxiangtu.top

[Q66] 行锁查询
来源：http://pwg.iojbl.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nly.shzxlz.cn

[Q67] 设置隔离级别
来源：http://eqd.cucudq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xhh.fanxiaobao.xyz

[Q68] 保存点
来源：http://xdo.chenzaomai.com

SAVEPOINT sp1;
来源：http://fbw.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://ukc.yvedp.cn

[Q69] 查看执行计划
来源：http://pid.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tft.wangshuangyany.cn

[Q70] 更新统计信息
来源：http://jkn.wangdashe.top

ANALYZE TABLE users;
来源：http://klm.hcnkem.com

[Q71] 查看建表语句
来源：http://vfm.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hyb.smart0.xyz

[Q72] 查看索引
来源：http://fus.meibo888.top

SHOW INDEX FROM users;
来源：http://wfu.hesvh.cn

[Q73] 查看表状态
来源：http://dhm.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rbk.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://wru.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lbx.tarul.cn

[Q75] 日期格式化
来源：http://bic.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ygi.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hlv.vehdjk.com

[Q76] 按天统计
来源：http://nzt.fengsongda.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zeg.0kj1m.cn

[Q77] 时间加减
来源：http://duj.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://awj.shanyushiyangtech.top

[Q78] 当前时间
来源：http://zwj.gzhubu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oww.bbcook.cn

[Q79] 字符串拼接
来源：http://ows.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ppn.cqqwz.cn

[Q80] 字符串截取
来源：http://spd.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pmq.cashguo.top

[Q81] 字符串替换
来源：http://juk.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cgq.cdnleiting.top

[Q82] 字符长度与字节长度
来源：http://kce.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bqg.zhixingplan.top

[Q83] 大小写转换
来源：http://nak.xylfe.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mrb.aizwys.cn

[Q84] 去除首尾空格
来源：http://rth.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://zdi.c1oappe.top

[Q85] 数值取整
来源：http://kza.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yad.tarul.cn

[Q86] 读取 JSON 字段
来源：http://nqo.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kjk.gogol.net.cn

[Q87] JSON 字段做条件
来源：http://qxm.ywan-chungtsiang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lsd.jqgfzy.top

[Q88] 行转列（条件聚合）
来源：http://enx.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ted.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mis.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://qdf.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cdn.gzhubu.top

[Q90] 生成序号列
来源：http://kxr.hammf.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ocn.sysykeji.top

================================================================================
来源：http://vpa.nanxuanxn.top

R. Bash 专题
来源：http://jlo.daxiang520.top

================================================================================
来源：http://wru.ydzc1.top

[R01] shebang 与严格模式
来源：http://hvm.ehwqpu.com

#!/usr/bin/env bash
来源：http://hcq.cheryme.top

set -euo pipefail
来源：http://rbc.chenzaomai.com

[R02] 变量赋值与使用
来源：http://cee.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://ioz.xziqi.cn

[R03] 只读变量
来源：http://gde.haohaochexian.top

readonly PI=3.14
来源：http://zok.fktsv.cn

[R04] 位置参数
来源：http://nse.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zqd.sweek.top

[R05] 参数默认值
来源：http://hzr.316326.xyz

name="${1:-default}"
来源：http://anf.tian-w.cn

[R06] 判断命令是否存在
来源：http://ztw.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eih.jqgfzy.top

[R07] if 判断文件
来源：http://gzo.zdbjq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://loy.bjfxy.top

[R08] 数值比较
来源：http://fdb.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ajw.cucudq.cn

[R09] 字符串比较
来源：http://xqt.zdbjq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mtp.ppjwa.cn

[R10] 正则匹配
来源：http://gqh.cdnleiting.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hro.yuxming.cn

[R11] case 多分支
来源：http://iiq.aibaodan.cn

case "$1" in
来源：http://fkh.yvedp.cn

start) echo "启动" ;;
来源：http://cia.ppjwa.cn

stop)  echo "停止" ;;
来源：http://buk.jianghu66.top

*)     echo "未知命令" ;;
来源：http://shm.jiagoushi.top

esac
来源：http://aom.daria6918.cn

[R12] for 遍历文件
来源：http://cbx.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://iyn.hammf.cn

[R13] for 计数循环
来源：http://kba.yonumen.top

for i in {1..10}; do echo "$i"; done
来源：http://srj.sjlbkw.cn

[R14] C 风格 for
来源：http://xcm.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qat.yonumen.top

[R15] while 逐行读文件
来源：http://xup.shanyushiyangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ntk.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://ltj.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gtm.mhx1999.top

[R17] 数组定义与取值
来源：http://cfy.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://qdf.havefunace.top

[R18] 遍历数组
来源：http://gdg.yangfankeji.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wni.ctjpmb.com

[R19] 数组长度
来源：http://edm.ctjpmb.com

echo "${#arr[@]}"
来源：http://xrq.sweek.top

[R20] 关联数组（字典）
来源：http://nxk.chenlongwang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jax.hnxiangtu.top

[R21] 字符串长度
来源：http://mqc.daxiang520.top

echo "${#s}"
来源：http://apz.ydjk.org.cn

[R22] 截取子串
来源：http://uun.fzhhl.top

echo "${s:0:5}"
来源：http://ofb.ctjpmb.com

[R23] 字符串替换
来源：http://udk.guowangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cdn.shanyushiyangtech.top

[R24] 大小写转换
来源：http://usm.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ied.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://afn.tian-w.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dtk.xuanzx.com

[R26] 命令替换
来源：http://lrp.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://pqu.tianlin.xyz

[R27] 算术展开
来源：http://xxa.jinqigfzy.top

echo $((1 + 2 * 3))
来源：http://bwo.fzhhl.top

[R28] 浮点运算
来源：http://tbr.sweek.top

echo "scale=2; 10/3" | bc
来源：http://pif.cashguo.top

[R29] 定义函数
来源：http://ndv.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lfg.jqgufenzy.top

[R30] 函数返回状态码
来源：http://rkt.jyoumei.cn

f() { return 0; }; f || echo "失败了"
来源：http://tsn.yanxiufei.cn

[R31] 局部变量
来源：http://czg.shangyingyoupin.top

f() { local x=1; echo "$x"; }
来源：http://rwe.xinyue.icu

[R32] 参数个数校验
来源：http://fhf.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bnf.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://fxa.jqgufenzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xny.jinqigufen.top

[R34] 退出时清理
来源：http://cal.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://uef.aizwys.cn

[R35] 后台执行并等待
来源：http://omu.hcnkem.com

sleep 5 & pid=$!; wait "$pid"
来源：http://zwu.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://zkb.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gzz.zycfv.cn

[R37] 把输出赋给变量
来源：http://hue.jqgfzy.top

files=$(ls -1)
来源：http://upc.wangshuangyany.cn

[R38] 管道串联
来源：http://adk.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://nnf.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://szr.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://upi.feifeiyinyue.top

[R40] 追加写日志
来源：http://yed.haohaochexian.top

echo "log" >> out.log
来源：http://vuy.sweek.top

[R41] 丢弃输出
来源：http://jrn.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://tux.vehdjk.com

[R42] 输入重定向
来源：http://zxe.cheryme.top

wc -l < a.txt
来源：http://tbf.tarul.cn

[R43] 按名字查找文件
来源：http://dkr.zhengqikj.top

find . -name "*.log" -type f
来源：http://rag.xinyue.icu

[R44] 按修改时间查找
来源：http://nia.ydzc1.top

find . -mtime -7 -type f
来源：http://pou.cucudq.cn

[R45] 批量删除
来源：http://tbv.jinqigufen.top

find . -name "*.tmp" -delete
来源：http://tnk.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://mmj.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qsk.yangfankeji.com

[R47] sed 单行替换
来源：http://zwl.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://vlg.guannengcc.top

[R48] awk 取指定列
来源：http://eht.jqgfzy.top

awk '{print $1, $3}' a.txt
来源：http://fsa.ybcxt.top

[R49] awk 带条件
来源：http://dlv.hammf.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bfm.sxryk.cn

[R50] awk 求和
来源：http://sku.hfpthk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sja.dashuyun.cn

[R51] 排序去重取前几
来源：http://bsj.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uys.nanxuanxn.top

[R52] 统计行数
来源：http://ioo.bbcook.cn

wc -l a.txt
来源：http://vqw.yj20258.top

[R53] 查看文件头与实时尾
来源：http://kgm.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eun.hongshengwenyu.top

[R54] 比较两个文件
来源：http://aek.yj20258888.top

diff a.txt b.txt
来源：http://iqy.yvedp.cn

[R55] 压缩与解压
来源：http://xmx.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ilp.sysykeji.top

[R56] 远程拷贝
来源：http://mwe.xuetiantiany.cn

scp file user@host:/path/
来源：http://wem.yuxming.cn

[R57] 远程执行命令
来源：http://wtp.gogol.net.cn

ssh user@host 'uptime'
来源：http://iav.dianchejie.cn

[R58] 下载文件
来源：http://wzp.shanyushiyangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qnt.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://ozt.gotoacloud.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xrl.jianghu66.top

[R60] 只看 HTTP 状态码
来源：http://nwd.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://khj.jiagoushi.top

[R61] 磁盘占用
来源：http://nvj.guowangkeji.top

df -h;  du -sh *
来源：http://ufe.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://rjo.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://nzg.gotoacloud.top

[R63] 内存与进程
来源：http://jnb.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://dcz.vehdjk.com

[R64] 结束进程
来源：http://xxh.dianchejie.cn

kill -9 $(pgrep -f app.py)
来源：http://cpx.nanxinkj.top

[R65] 查看端口占用
来源：http://llg.sweek.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aeh.epnwcf.com

[R66] 定时任务
来源：http://bli.shzxlz.cn

crontab -e;  crontab -l
来源：http://gcy.shuidangran.top

[R67] 生成随机十六进制串
来源：http://fwa.gaohongyu789.top

openssl rand -hex 16
来源：http://gmj.sufxvd.cn

[R68] 计算文件校验值
来源：http://okk.zhixingplan.top

sha256sum a.txt;  md5sum a.txt
来源：http://pro.ctjpmb.com

[R69] 生成随机密码
来源：http://rkk.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://dwk.chenzaomai.com

[R70] 时间戳与互转
来源：http://nyz.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://ipj.pycfn.com

[R71] 日期格式化
来源：http://luw.pengpengdd.cyou

date +"%Y-%m-%d %H:%M:%S"
来源：http://cxr.sjlbkw.cn

[R72] 等待端口就绪
来源：http://xeb.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://huh.yvedp.cn

[R73] 分割大日志
来源：http://dzd.nanxuanxn.top

split -l 1000 big.log part_
来源：http://lay.vehdjk.com

[R74] 批量重命名
来源：http://rhp.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kpr.bjfxy.top

[R75] 导出环境变量
来源：http://dfo.hywenlv.cn

export PATH="$HOME/bin:$PATH"
来源：http://ifq.hnqzz.top

[R76] 使用临时文件
来源：http://flx.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pvo.dashuyun.cn

[R77] 读取用户输入
来源：http://egb.jiagoushi.top


<!-- 参考信息 -->