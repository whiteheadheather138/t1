代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dnr.guowangkeji.top

[Q26] 计数
来源：http://qsz.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://hkh.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://hho.smart0.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jcg.hesvh.cn

[Q28] 求和与平均
来源：http://mty.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xie.tianlin.xyz

[Q29] 最大最小值
来源：http://yxx.dianchejie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dlq.shuidangran.top

[Q30] 分组统计
来源：http://ojd.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://amk.yuanzhike.top

[Q31] 分组后过滤
来源：http://noa.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eja.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://iaz.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://plq.sysykeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://voc.c1oappe.top

[Q33] 多列分组
来源：http://qgx.sxryk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://szk.kuanghao11.cn

[Q34] 每组取第一条
来源：http://art.ivvv.top

SELECT * FROM (
来源：http://tev.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gvt.cdnleiting.top

) t WHERE rn = 1;
来源：http://asn.xziqi.cn

[Q35] 内连接
来源：http://wyi.sjlbkw.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dil.haohaochexian.top

[Q36] 左连接
来源：http://iiw.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hmj.hongshengwenyu.top

[Q37] 右连接
来源：http://tiq.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sqz.sxryk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iju.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mwy.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://crp.zhixingplan.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://evs.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yga.vehdjk.com

[Q40] 交叉连接（笛卡尔积）
来源：http://byv.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uqi.yanxiufei.cn

[Q41] 多表连接
来源：http://lmt.cdnleiting.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wac.dianchejie.cn

JOIN users u ON u.id = o.user_id
来源：http://hwy.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://sav.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://bor.chenzaomai.com

SELECT u.name, o.amount FROM users u
来源：http://qrl.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gkn.jqgfzy.top

[Q43] 标量子查询
来源：http://fnx.jinqigufen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kri.shangyingyoupin.top

[Q44] IN 子查询
来源：http://jib.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ztq.tian-w.cn

[Q45] EXISTS 判断存在
来源：http://ptk.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vkw.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://dzc.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ibd.xuetiantiany.cn

[Q47] 与平均值比较
来源：http://qne.sxryk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://upk.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://lqu.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dhi.bbcook.cn

SELECT * FROM t WHERE c > 5;
来源：http://ebv.fengsongda.top

[Q49] 更新单行
来源：http://tji.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fzi.yj20258.top

[Q50] 批量更新
来源：http://uac.hnxiangtu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ynb.gzhubu.top

[Q51] 用子查询更新
来源：http://mya.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://azz.fengsongda.top

[Q52] 删除指定行
来源：http://vwb.tian-w.cn

DELETE FROM users WHERE id = 10;
来源：http://xse.jinqigfzy.top

[Q53] 按条件删除
来源：http://ykl.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cjc.zhoulong.xyz

[Q54] 清空表
来源：http://xxb.hfpthk.cn

TRUNCATE TABLE logs;
来源：http://gla.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://tle.hfpthk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gss.ydzc1.top

[Q56] 密集排名（并列不占位）
来源：http://gze.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mvo.jinqigfzy.top

[Q57] 行号
来源：http://nee.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tyv.cucudq.cn

[Q58] 累计求和
来源：http://kmm.nanxinkj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://shf.ydzc1.top

[Q59] 分组内累计
来源：http://owd.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uaq.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://hpm.chenjidiqi.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hoo.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bip.sysykeji.top

[Q61] 移动平均
来源：http://erd.sxryk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mtn.hcnkem.com

[Q62] 分组占比
来源：http://qwe.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zww.wangshuangyany.cn

[Q63] 开启事务
来源：http://olb.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jba.vehdjk.com

[Q64] 提交事务
来源：http://eui.shangyingyoupin.top

COMMIT;
来源：http://idw.hongshengwenyu.top

[Q65] 回滚事务
来源：http://anq.jinyuanbaomall.cn

ROLLBACK;
来源：http://ftj.jinghuilouyu.cn

[Q66] 行锁查询
来源：http://wfg.svipenyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://igg.nanxuanxn.top

[Q67] 设置隔离级别
来源：http://npn.shzxlz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://icw.ctjpmb.com

[Q68] 保存点
来源：http://vfl.vehdjk.com

SAVEPOINT sp1;
来源：http://xad.yvedp.cn

ROLLBACK TO sp1;
来源：http://hjd.wangdashe.top

[Q69] 查看执行计划
来源：http://xlg.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kok.0kj1m.cn

[Q70] 更新统计信息
来源：http://uwl.shuidangran.top

ANALYZE TABLE users;
来源：http://bzz.cucudq.cn

[Q71] 查看建表语句
来源：http://hfs.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://enh.nanxuanxn.top

[Q72] 查看索引
来源：http://gpd.jqgufenzy.top

SHOW INDEX FROM users;
来源：http://qij.shangyingyoupin.top

[Q73] 查看表状态
来源：http://kxg.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://bcu.jianghu66.top

[Q74] 强制使用索引
来源：http://lpx.hesvh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mcd.yj20258888.top

[Q75] 日期格式化
来源：http://cyj.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jwq.kuanghao11.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rox.cucudq.cn

[Q76] 按天统计
来源：http://pyb.yangfankeji.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zel.yj202588.top

[Q77] 时间加减
来源：http://kih.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kis.yj202588.top

[Q78] 当前时间
来源：http://emn.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nck.cdnleiting.top

[Q79] 字符串拼接
来源：http://uik.yfazqb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://evo.epnwcf.com

[Q80] 字符串截取
来源：http://sda.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://klk.ppjwa.cn

[Q81] 字符串替换
来源：http://qaw.meibo888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cbl.yangfankeji.com

[Q82] 字符长度与字节长度
来源：http://abu.cheryme.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://roo.316326.xyz

[Q83] 大小写转换
来源：http://mwk.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fgc.tanke756.top

[Q84] 去除首尾空格
来源：http://qzj.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://lqu.meibo888.top

[Q85] 数值取整
来源：http://oax.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://emm.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://kht.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qtz.bjfxy.top

[Q87] JSON 字段做条件
来源：http://tsm.zhongyouzk.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cig.haohaochexian.top

[Q88] 行转列（条件聚合）
来源：http://ann.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hwt.kuanghao11.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://udm.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://pzq.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lci.havefunace.top

[Q90] 生成序号列
来源：http://qcr.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lig.nanxinkj.top

================================================================================
来源：http://qlf.svipenyu.cn

R. Bash 专题
来源：http://ysu.hfpthk.cn

================================================================================
来源：http://fco.pycfn.com

[R01] shebang 与严格模式
来源：http://ylv.quarkkingdee.top

#!/usr/bin/env bash
来源：http://izu.xylfe.cn

set -euo pipefail
来源：http://lrk.redwolf501.top

[R02] 变量赋值与使用
来源：http://csw.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://hjw.hnqzz.top

[R03] 只读变量
来源：http://wlr.jlsjyb.cn

readonly PI=3.14
来源：http://jvq.ywan-chungtsiang.top

[R04] 位置参数
来源：http://tfs.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zxd.shuidangran.top

[R05] 参数默认值
来源：http://jlo.hesvh.cn

name="${1:-default}"
来源：http://rgh.redwolf501.top

[R06] 判断命令是否存在
来源：http://bxk.hcnkem.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zox.yj20258.top

[R07] if 判断文件
来源：http://oef.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zhu.jianghu66.top

[R08] 数值比较
来源：http://dfb.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ray.ydzc1.top

[R09] 字符串比较
来源：http://gwc.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://plm.zdbjq.cn

[R10] 正则匹配
来源：http://zzs.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://owj.zhongyouzk.top

[R11] case 多分支
来源：http://rva.pycfn.com

case "$1" in
来源：http://gzh.c1oappe.top

start) echo "启动" ;;
来源：http://fjn.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://swx.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://vmy.wangshuangyany.cn

esac
来源：http://ldx.dianchejie.cn

[R12] for 遍历文件
来源：http://zok.yonumen.top

for f in *.txt; do echo "$f"; done
来源：http://omr.jinghuilouyu.cn

[R13] for 计数循环
来源：http://jwa.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://ehd.jinghuilouyu.cn

[R14] C 风格 for
来源：http://hqg.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yfd.cheryme.top

[R15] while 逐行读文件
来源：http://hqa.andypj.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ygs.jiagoushi.top

[R16] until 等待条件
来源：http://byd.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jxg.ydjk.org.cn

[R17] 数组定义与取值
来源：http://jkx.haohaochexian.top

arr=(a b c); echo "${arr[0]}"
来源：http://wao.ybcxt.top

[R18] 遍历数组
来源：http://hmj.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jet.dianchejie.cn

[R19] 数组长度
来源：http://xmq.xziqi.cn

echo "${#arr[@]}"
来源：http://eiu.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://cwg.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ehe.yj20258.top

[R21] 字符串长度
来源：http://bfl.yj20258888.top

echo "${#s}"
来源：http://fsk.tarul.cn

[R22] 截取子串
来源：http://mbu.52xcode.cn

echo "${s:0:5}"
来源：http://rqn.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://uud.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hlj.yueranfly.top

[R24] 大小写转换
来源：http://gfs.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://evd.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://sms.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://nuv.hysaishi.cn

[R26] 命令替换
来源：http://elr.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://vqf.cqqwz.cn

[R27] 算术展开
来源：http://upv.hfpthk.cn

echo $((1 + 2 * 3))
来源：http://vcm.smart0.xyz

[R28] 浮点运算
来源：http://hpp.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://hsp.nanxuanxn.top

[R29] 定义函数
来源：http://nco.sysykeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rxi.xylfe.cn

[R30] 函数返回状态码
来源：http://xlm.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://sfo.quarkkingdee.top

[R31] 局部变量
来源：http://gaa.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://xos.guowangkeji.top

[R32] 参数个数校验
来源：http://ecj.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pek.yonumen.top

[R33] 捕获错误并提示行号
来源：http://yyd.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ylq.52xcode.cn

[R34] 退出时清理
来源：http://bui.yangfankeji.com

trap 'rm -f "$tmp"' EXIT
来源：http://fkm.chenzaomai.com

[R35] 后台执行并等待
来源：http://zgf.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://got.zycfv.cn

[R36] 并发执行多个任务
来源：http://qaj.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xbl.dashuyun.cn

[R37] 把输出赋给变量
来源：http://ziv.hesvh.cn

files=$(ls -1)
来源：http://mor.jqgfzy.top

[R38] 管道串联
来源：http://iqg.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://jzz.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://pnw.havefunace.top

cmd > out.log 2>&1
来源：http://dzb.fzhhl.top

[R40] 追加写日志
来源：http://mbb.hnqzz.top

echo "log" >> out.log
来源：http://yil.nwbrower.top

[R41] 丢弃输出
来源：http://luq.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://fzm.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://qoz.quarkkingdee.top

wc -l < a.txt
来源：http://qjm.xinyue.icu

[R43] 按名字查找文件
来源：http://eov.zhoulong.xyz

find . -name "*.log" -type f
来源：http://seh.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://qoc.hcnkem.com

find . -mtime -7 -type f
来源：http://ruv.hcnkem.com

[R45] 批量删除
来源：http://acr.cashguo.top

find . -name "*.tmp" -delete
来源：http://myq.chenzaomai.com

[R46] 递归替换文件内容
来源：http://swh.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://utt.nanxinkj.top

[R47] sed 单行替换
来源：http://fxr.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lfq.sweek.top

[R48] awk 取指定列
来源：http://clx.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://zoi.hywenlv.cn

[R49] awk 带条件
来源：http://zlw.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://krp.cashguo.top

[R50] awk 求和
来源：http://yrw.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://wbd.epnwcf.com

[R51] 排序去重取前几
来源：http://yvg.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zmw.meibo888.top

[R52] 统计行数
来源：http://ujx.fktsv.cn

wc -l a.txt
来源：http://bgg.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://zwh.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ttm.sysykeji.top

[R54] 比较两个文件
来源：http://aaz.chenlongwang.top

diff a.txt b.txt
来源：http://bdq.cqqwz.cn

[R55] 压缩与解压
来源：http://mzl.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mcg.fehbvm.com

[R56] 远程拷贝
来源：http://hrf.ivvv.top

scp file user@host:/path/
来源：http://wtb.nanxuanxn.top

[R57] 远程执行命令
来源：http://yuf.yonumen.top

ssh user@host 'uptime'
来源：http://eqg.cashguo.top

[R58] 下载文件
来源：http://uap.xziqi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://whp.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://llo.xziqi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mqx.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://pve.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qfz.tianlin.xyz

[R61] 磁盘占用
来源：http://ekj.guannengcc.top

df -h;  du -sh *
来源：http://kwb.c1oappe.top

[R62] 找最占空间的文件
来源：http://tvz.ydjk.org.cn

du -ah . | sort -rh | head -10
来源：http://gzj.shanyushiyangtech.top

[R63] 内存与进程
来源：http://obk.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://pnz.cucudq.cn

[R64] 结束进程
来源：http://foy.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://giw.nanxinkj.top

[R65] 查看端口占用
来源：http://wps.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bhl.xuetiantiany.cn

[R66] 定时任务
来源：http://ktu.xinyue.icu

crontab -e;  crontab -l
来源：http://zuu.sysykeji.top

[R67] 生成随机十六进制串
来源：http://vbq.yj202588.top

openssl rand -hex 16
来源：http://thf.yangfankeji.com

[R68] 计算文件校验值
来源：http://huh.hywenlv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ntj.sxryk.cn

[R69] 生成随机密码
来源：http://yqc.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://dvg.ybcxt.top

[R70] 时间戳与互转
来源：http://ccp.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://vsz.quarkkingdee.top

[R71] 日期格式化
来源：http://lpd.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nlf.nanxinkj.top

[R72] 等待端口就绪
来源：http://sbn.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://gio.pengpengdd.cyou

[R73] 分割大日志
来源：http://axm.gogol.net.cn

split -l 1000 big.log part_
来源：http://xjy.yj20258.top

[R74] 批量重命名
来源：http://svl.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fyz.guowangkeji.top

[R75] 导出环境变量
来源：http://kmi.bbcook.cn


<!-- 参考信息 -->