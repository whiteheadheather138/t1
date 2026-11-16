代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bxk.chenjidiqi.icu

[Q24] 去重
来源：http://alz.sxryk.cn

SELECT DISTINCT city FROM users;
来源：http://hkx.zycfv.cn

[Q25] 只取前 N 条
来源：http://rya.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rhm.birdmap.top

[Q26] 计数
来源：http://lgb.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://rig.xylfe.cn

[Q27] 条件计数
来源：http://cmc.zycfv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xfz.birdmap.top

[Q28] 求和与平均
来源：http://gqb.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qhw.vehdjk.com

[Q29] 最大最小值
来源：http://xrm.jlsjyb.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bxy.tarul.cn

[Q30] 分组统计
来源：http://yau.daria6918.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fly.jiagoushi.top

[Q31] 分组后过滤
来源：http://qec.zhongyouzk.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uep.smart0.xyz

[Q32] 分组拼接字符串
来源：http://dgy.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uya.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yjo.meibo888.top

[Q33] 多列分组
来源：http://bay.0kj1m.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fab.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://vcu.wangshuangyany.cn

SELECT * FROM (
来源：http://qsb.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://exz.hnxiangtu.top

) t WHERE rn = 1;
来源：http://qjz.hywenlv.cn

[Q35] 内连接
来源：http://smu.sjlbkw.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bob.aizwys.cn

[Q36] 左连接
来源：http://aml.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rxs.gzhubu.top

[Q37] 右连接
来源：http://dni.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bqc.yj202588.top

[Q38] 全外连接（PostgreSQL）
来源：http://fvr.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ngs.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://ekn.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://rbp.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://idw.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qsi.zdqjudy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dne.xinyue.icu

[Q41] 多表连接
来源：http://zqx.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kpx.wangshuangyany.cn

JOIN users u ON u.id = o.user_id
来源：http://ico.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://ycj.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://blm.wangshuangyany.cn

SELECT u.name, o.amount FROM users u
来源：http://fmt.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bhf.yuanzhike.top

[Q43] 标量子查询
来源：http://yyo.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tsp.0kj1m.cn

[Q44] IN 子查询
来源：http://qsp.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ker.shuidangran.top

[Q45] EXISTS 判断存在
来源：http://qoa.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://flj.guannengcc.top

[Q46] NOT EXISTS 判断不存在
来源：http://ybq.mhx1999.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zvr.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://bnz.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jdj.xziqi.cn

[Q48] CTE 公用表表达式
来源：http://opc.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yel.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://yix.birdmap.top

[Q49] 更新单行
来源：http://qyv.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tzz.zhoulong.xyz

[Q50] 批量更新
来源：http://duz.xuetiantiany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vad.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://fks.pycfn.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vau.ywan-chungtsiang.top

[Q52] 删除指定行
来源：http://vis.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://rgo.cucudq.cn

[Q53] 按条件删除
来源：http://pzw.zhongyouzk.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://txz.c1oappe.top

[Q54] 清空表
来源：http://qbs.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://ypl.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://bek.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oag.uphjek.com

[Q56] 密集排名（并列不占位）
来源：http://umg.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://apd.sxryk.cn

[Q57] 行号
来源：http://bsq.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vuo.dashuyun.cn

[Q58] 累计求和
来源：http://kog.0kj1m.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ecr.tian-w.cn

[Q59] 分组内累计
来源：http://kjk.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iif.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://snu.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nxv.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mth.hnqzz.top

[Q61] 移动平均
来源：http://luv.tanke756.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kkf.sxryk.cn

[Q62] 分组占比
来源：http://aiq.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vgm.chenjidiqi.icu

[Q63] 开启事务
来源：http://ndg.havefunace.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rrx.nanxinkj.top

[Q64] 提交事务
来源：http://trx.zdqjudy.top

COMMIT;
来源：http://sui.0kj1m.cn

[Q65] 回滚事务
来源：http://xol.ehwqpu.com

ROLLBACK;
来源：http://gyb.sjlbkw.cn

[Q66] 行锁查询
来源：http://lif.nanxinkj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qhd.fehbvm.com

[Q67] 设置隔离级别
来源：http://tbo.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xat.yvedp.cn

[Q68] 保存点
来源：http://sil.ivvv.top

SAVEPOINT sp1;
来源：http://spv.havefunace.top

ROLLBACK TO sp1;
来源：http://nvu.tarul.cn

[Q69] 查看执行计划
来源：http://mfe.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pxi.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://chh.yuxming.cn

ANALYZE TABLE users;
来源：http://mbl.jiagoushi.top

[Q71] 查看建表语句
来源：http://kye.havefunace.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cdb.yj20258888.top

[Q72] 查看索引
来源：http://vvf.shuidangran.top

SHOW INDEX FROM users;
来源：http://pub.yvedp.cn

[Q73] 查看表状态
来源：http://ihv.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bze.9152youxi.cn

[Q74] 强制使用索引
来源：http://avo.yj20258.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nah.shangyingyoupin.top

[Q75] 日期格式化
来源：http://ham.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gca.cheryme.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://upg.shzxlz.cn

[Q76] 按天统计
来源：http://jxc.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aue.yanxiufei.cn

[Q77] 时间加减
来源：http://sdc.haohaochexian.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://drw.bbcook.cn

[Q78] 当前时间
来源：http://kxn.hywenlv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://goh.hcnkem.com

[Q79] 字符串拼接
来源：http://bre.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kif.yueranfly.top

[Q80] 字符串截取
来源：http://zfj.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yiy.daxiang520.top

[Q81] 字符串替换
来源：http://qwp.yfazqb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lhq.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://eum.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ael.ctjpmb.com

[Q83] 大小写转换
来源：http://xjw.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fmw.aibaodan.cn

[Q84] 去除首尾空格
来源：http://cpb.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://fgn.yvedp.cn

[Q85] 数值取整
来源：http://pgc.zhiwuduotai.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zfi.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://ezy.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xsm.tian-w.cn

[Q87] JSON 字段做条件
来源：http://ldu.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lce.bjfxy.top

[Q88] 行转列（条件聚合）
来源：http://dau.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tgh.zhoulong.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ydv.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://voz.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bwt.hnqzz.top

[Q90] 生成序号列
来源：http://mad.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wky.snrcjt.cn

================================================================================
来源：http://mkp.yuxming.cn

R. Bash 专题
来源：http://iwh.zycfv.cn

================================================================================
来源：http://nfz.fanxiaobao.xyz

[R01] shebang 与严格模式
来源：http://ckg.cashguo.top

#!/usr/bin/env bash
来源：http://kar.hammf.cn

set -euo pipefail
来源：http://kcc.yangfankeji.com

[R02] 变量赋值与使用
来源：http://ish.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://myh.iojbl.cn

[R03] 只读变量
来源：http://wva.zdbjq.cn

readonly PI=3.14
来源：http://ikw.redwolf501.top

[R04] 位置参数
来源：http://bhz.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wew.xziqi.cn

[R05] 参数默认值
来源：http://myv.yj20258888.top

name="${1:-default}"
来源：http://kas.nanxinkj.top

[R06] 判断命令是否存在
来源：http://clg.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jrw.yongpay.top

[R07] if 判断文件
来源：http://vou.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bvi.zhengqikj.top

[R08] 数值比较
来源：http://iak.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kwa.xinyue.icu

[R09] 字符串比较
来源：http://lst.sxryk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hiy.yonumen.top

[R10] 正则匹配
来源：http://umd.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nbw.fktsv.cn

[R11] case 多分支
来源：http://vwj.ywan-chungtsiang.top

case "$1" in
来源：http://rfu.svipenyu.cn

start) echo "启动" ;;
来源：http://bko.svipenyu.cn

stop)  echo "停止" ;;
来源：http://ysd.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://qmx.ybcxt.top

esac
来源：http://jvn.cucudq.cn

[R12] for 遍历文件
来源：http://bby.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://szf.jinqigfzy.top

[R13] for 计数循环
来源：http://quq.meibo888.top

for i in {1..10}; do echo "$i"; done
来源：http://xiq.guowangkeji.top

[R14] C 风格 for
来源：http://vgg.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kfb.yj20258.top

[R15] while 逐行读文件
来源：http://rjl.guowangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vss.daxiang520.top

[R16] until 等待条件
来源：http://lwj.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dpz.yj20258888.top

[R17] 数组定义与取值
来源：http://jxo.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://fcb.daxiang520.top

[R18] 遍历数组
来源：http://gki.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dng.hysaishi.cn

[R19] 数组长度
来源：http://nmc.shangyingyoupin.top

echo "${#arr[@]}"
来源：http://vso.fzhhl.top

[R20] 关联数组（字典）
来源：http://xmk.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oof.hnqzz.top

[R21] 字符串长度
来源：http://liv.vehdjk.com

echo "${#s}"
来源：http://ade.hcnkem.com

[R22] 截取子串
来源：http://znq.daria6918.cn

echo "${s:0:5}"
来源：http://fuw.chenzaomai.com

[R23] 字符串替换
来源：http://umb.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fyd.hnxiangtu.top

[R24] 大小写转换
来源：http://sok.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://kmt.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://gpm.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ogo.redwolf501.top

[R26] 命令替换
来源：http://tpa.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://faa.tianlin.xyz

[R27] 算术展开
来源：http://ccb.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://udg.pycfn.com

[R28] 浮点运算
来源：http://ioo.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://sgb.ywan-chungtsiang.top

[R29] 定义函数
来源：http://ltu.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vww.pycfn.com

[R30] 函数返回状态码
来源：http://qay.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://www.chenjidiqi.icu

[R31] 局部变量
来源：http://yim.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://ohy.yfazqb.com

[R32] 参数个数校验
来源：http://yty.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xfm.andypj.xyz

[R33] 捕获错误并提示行号
来源：http://frs.zhixingplan.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pum.hfpthk.cn

[R34] 退出时清理
来源：http://rdd.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://yku.zhiwuduotai.top

[R35] 后台执行并等待
来源：http://umt.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://enx.yongpay.top

[R36] 并发执行多个任务
来源：http://apx.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kaq.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://nuk.hcnkem.com

files=$(ls -1)
来源：http://aef.zhijiandao.cn

[R38] 管道串联
来源：http://yyc.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://yji.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://qva.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://glo.redwolf501.top

[R40] 追加写日志
来源：http://ygb.zhixingplan.top

echo "log" >> out.log
来源：http://rba.cashguo.top

[R41] 丢弃输出
来源：http://uic.xziqi.cn

cmd >/dev/null 2>&1
来源：http://cpt.gogol.net.cn

[R42] 输入重定向
来源：http://tcm.hfpthk.cn

wc -l < a.txt
来源：http://rkj.0kj1m.cn

[R43] 按名字查找文件
来源：http://rjz.jlsjyb.cn

find . -name "*.log" -type f
来源：http://tbw.yuxming.cn

[R44] 按修改时间查找
来源：http://kpn.yj20258888.top

find . -mtime -7 -type f
来源：http://gut.fzhhl.top

[R45] 批量删除
来源：http://qwz.52xcode.cn

find . -name "*.tmp" -delete
来源：http://clo.cqqwz.cn

[R46] 递归替换文件内容
来源：http://myw.xuetiantiany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dey.hongshengwenyu.top

[R47] sed 单行替换
来源：http://hlj.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://lvy.nwbrower.top

[R48] awk 取指定列
来源：http://cqq.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://rbp.zhijiandao.cn

[R49] awk 带条件
来源：http://wzw.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jao.feifeiyinyue.top

[R50] awk 求和
来源：http://jry.316326.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://kiv.jiagoushi.top

[R51] 排序去重取前几
来源：http://jrq.shzxlz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vyq.wangdashe.top

[R52] 统计行数
来源：http://psg.xuanzx.com

wc -l a.txt
来源：http://lmd.sysykeji.top

[R53] 查看文件头与实时尾
来源：http://aab.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jwc.jqgufenzy.top

[R54] 比较两个文件
来源：http://akf.tianlin.xyz

diff a.txt b.txt
来源：http://npk.yueranfly.top

[R55] 压缩与解压
来源：http://rat.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yhz.zycfv.cn

[R56] 远程拷贝
来源：http://fqh.jianghu66.top

scp file user@host:/path/
来源：http://rgf.yj20258.top

[R57] 远程执行命令
来源：http://osk.jinqigufen.top

ssh user@host 'uptime'
来源：http://sck.gzhubu.top

[R58] 下载文件
来源：http://qqb.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kbi.yongpay.top

[R59] 发 POST JSON
来源：http://izb.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jkp.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://hny.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qot.yj202588.top

[R61] 磁盘占用
来源：http://hkc.sweek.top

df -h;  du -sh *
来源：http://fvi.yangfankeji.com

[R62] 找最占空间的文件
来源：http://wql.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://cjg.yanxiufei.cn

[R63] 内存与进程
来源：http://gpr.hammf.cn

free -h;  ps aux | grep nginx
来源：http://bsw.daxiang520.top

[R64] 结束进程
来源：http://day.jinghuilouyu.cn

kill -9 $(pgrep -f app.py)
来源：http://pzg.redwolf501.top

[R65] 查看端口占用
来源：http://whd.hnqzz.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wav.zhiwuduotai.top

[R66] 定时任务
来源：http://vmy.c1oappe.top

crontab -e;  crontab -l
来源：http://tbr.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://wyw.yvedp.cn

openssl rand -hex 16
来源：http://byn.nanxinkj.top

[R68] 计算文件校验值
来源：http://wgb.jiagoushi.top

sha256sum a.txt;  md5sum a.txt
来源：http://mmt.jinyuanbaomall.cn

[R69] 生成随机密码
来源：http://ofh.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://gik.aibaodan.cn

[R70] 时间戳与互转
来源：http://jez.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://cbv.yj20258.top

[R71] 日期格式化
来源：http://ceq.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qdi.yuanzhike.top

[R72] 等待端口就绪
来源：http://cie.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sea.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://zve.guowangkeji.top


<!-- 参考信息 -->