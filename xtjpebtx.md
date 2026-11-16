代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://pko.shanyushiyangkeji.top

[Q22] 排序
来源：http://dch.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dcw.jiagoushi.top

[Q23] 分页
来源：http://gnn.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lvh.hammf.cn

[Q24] 去重
来源：http://fdq.xuanzx.com

SELECT DISTINCT city FROM users;
来源：http://vbd.fzhhl.top

[Q25] 只取前 N 条
来源：http://fax.nanxuanxn.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ktu.sufxvd.cn

[Q26] 计数
来源：http://ltw.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://oec.smart0.xyz

[Q27] 条件计数
来源：http://fnd.yangfankeji.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iaz.shanyushiyangkeji.top

[Q28] 求和与平均
来源：http://ttg.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://clg.zdqjudy.top

[Q29] 最大最小值
来源：http://ccy.hesvh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cxr.gzhubu.top

[Q30] 分组统计
来源：http://uqg.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ybm.zycfv.cn

[Q31] 分组后过滤
来源：http://dsw.redwolf501.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kis.birdmap.top

[Q32] 分组拼接字符串
来源：http://mhu.zhixingplan.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cwu.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eth.cdnleiting.top

[Q33] 多列分组
来源：http://ucw.dianchejie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tld.sweek.top

[Q34] 每组取第一条
来源：http://qfj.gogol.net.cn

SELECT * FROM (
来源：http://zhw.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qvp.hnqzz.top

) t WHERE rn = 1;
来源：http://eay.chenjidiqi.icu

[Q35] 内连接
来源：http://epv.cqqwz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rtm.feifeiyinyue.top

[Q36] 左连接
来源：http://mrr.zdqjudy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mhn.jinghuilouyu.cn

[Q37] 右连接
来源：http://qiv.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vvo.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tdw.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://etf.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://gux.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bra.yfazqb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iqg.chenlongwang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eoa.jinyuanbaomall.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bem.yj202588.top

[Q41] 多表连接
来源：http://ywi.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tqs.yonumen.top

JOIN users u ON u.id = o.user_id
来源：http://gqq.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://xbb.svipenyu.cn

[Q42] 连接条件附加过滤
来源：http://hmi.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://btp.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ojn.yuxming.cn

[Q43] 标量子查询
来源：http://fwd.gogol.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eah.jinqigufen.top

[Q44] IN 子查询
来源：http://uee.birdmap.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vrv.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://ekh.cucudq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://het.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vlb.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qpt.pycfn.com

[Q47] 与平均值比较
来源：http://kpj.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vpz.yj20258.top

[Q48] CTE 公用表表达式
来源：http://oxb.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fij.chenlongwang.top

SELECT * FROM t WHERE c > 5;
来源：http://bvw.sweek.top

[Q49] 更新单行
来源：http://bsx.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gfz.xuanzx.com

[Q50] 批量更新
来源：http://iiy.tian-w.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wps.jiagoushi.top

[Q51] 用子查询更新
来源：http://ykf.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bzz.dianchejie.cn

[Q52] 删除指定行
来源：http://ypf.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://omx.epnwcf.com

[Q53] 按条件删除
来源：http://hwe.yuanzhike.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nns.nanxinkj.top

[Q54] 清空表
来源：http://krl.shuidangran.top

TRUNCATE TABLE logs;
来源：http://gjw.sufxvd.cn

[Q55] 排名（并列占位）
来源：http://xej.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gkb.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://gak.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vca.feifeiyinyue.top

[Q57] 行号
来源：http://roj.ivvv.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mnp.nanxinkj.top

[Q58] 累计求和
来源：http://riu.fktsv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jat.daxiang520.top

[Q59] 分组内累计
来源：http://ctw.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://loz.cdnleiting.top

[Q60] 取上一行 / 下一行
来源：http://ndq.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://djl.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jtw.iojbl.cn

[Q61] 移动平均
来源：http://uyo.aibaodan.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ohs.yanxiufei.cn

[Q62] 分组占比
来源：http://ngn.xinyue.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xyv.yuanzhike.top

[Q63] 开启事务
来源：http://qfg.havefunace.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pbq.zdbjq.cn

[Q64] 提交事务
来源：http://yam.ctjpmb.com

COMMIT;
来源：http://eoa.tian-w.cn

[Q65] 回滚事务
来源：http://liq.gogol.net.cn

ROLLBACK;
来源：http://svl.xuetiantiany.cn

[Q66] 行锁查询
来源：http://cgr.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zaw.zhixingplan.top

[Q67] 设置隔离级别
来源：http://mmo.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rty.tian-w.cn

[Q68] 保存点
来源：http://hoj.hnqzz.top

SAVEPOINT sp1;
来源：http://xaj.dashuyun.cn

ROLLBACK TO sp1;
来源：http://bmh.fzhhl.top

[Q69] 查看执行计划
来源：http://yya.aibaodan.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qbl.shangyingyoupin.top

[Q70] 更新统计信息
来源：http://qkc.316326.xyz

ANALYZE TABLE users;
来源：http://hdr.birdmap.top

[Q71] 查看建表语句
来源：http://avg.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tgm.smart0.xyz

[Q72] 查看索引
来源：http://cok.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://hem.cheryme.top

[Q73] 查看表状态
来源：http://vcz.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zqq.aizwys.cn

[Q74] 强制使用索引
来源：http://cov.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pas.9152youxi.cn

[Q75] 日期格式化
来源：http://uyc.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tvi.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gxe.shuidangran.top

[Q76] 按天统计
来源：http://qeh.xinyue.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nfw.shanyushiyangtech.top

[Q77] 时间加减
来源：http://ojv.fengsongda.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iqq.hywenlv.cn

[Q78] 当前时间
来源：http://nnq.hfpthk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xvc.guannengcc.top

[Q79] 字符串拼接
来源：http://gzi.shangyingyoupin.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://adp.tianlin.xyz

[Q80] 字符串截取
来源：http://igj.xinyue.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ziy.zhoulong.xyz

[Q81] 字符串替换
来源：http://agb.jinqigfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pni.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://uee.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rwk.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://cdd.jiagoushi.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ayq.aizwys.cn

[Q84] 去除首尾空格
来源：http://pnw.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://xie.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://akf.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jcv.daxiang520.top

[Q86] 读取 JSON 字段
来源：http://dkv.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pbm.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://dfm.hywenlv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kzv.xingfuxueyuan.xyz

[Q88] 行转列（条件聚合）
来源：http://gea.yvedp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://afv.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pwk.cqqwz.cn

[Q89] 判断表是否存在
来源：http://ouq.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ncw.tarul.cn

[Q90] 生成序号列
来源：http://uui.chenzaomai.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jsg.cdnleiting.top

================================================================================
来源：http://zxy.birdmap.top

R. Bash 专题
来源：http://fka.zdbjq.cn

================================================================================
来源：http://dkj.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://tht.tianlin.xyz

#!/usr/bin/env bash
来源：http://kom.tianlin.xyz

set -euo pipefail
来源：http://hvd.redwolf501.top

[R02] 变量赋值与使用
来源：http://jek.wangdashe.top

name="Tom"; echo "$name"
来源：http://tjx.jqgfzy.top

[R03] 只读变量
来源：http://otj.ydjk.org.cn

readonly PI=3.14
来源：http://gnz.shanyushiyangtech.top

[R04] 位置参数
来源：http://npi.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rog.tian-w.cn

[R05] 参数默认值
来源：http://tra.havefunace.top

name="${1:-default}"
来源：http://kgi.yuanzhike.top

[R06] 判断命令是否存在
来源：http://vfy.tarul.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jtn.zdqjudy.top

[R07] if 判断文件
来源：http://ajb.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qqs.jinqigfzy.top

[R08] 数值比较
来源：http://hbp.daxiang520.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gbf.zhoulong.xyz

[R09] 字符串比较
来源：http://ytl.c1oappe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fee.9152youxi.cn

[R10] 正则匹配
来源：http://tvg.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ogo.yfazqb.com

[R11] case 多分支
来源：http://jun.nwbrower.top

case "$1" in
来源：http://upz.sufxvd.cn

start) echo "启动" ;;
来源：http://dym.jyoumei.cn

stop)  echo "停止" ;;
来源：http://mfx.zdqjudy.top

*)     echo "未知命令" ;;
来源：http://qlw.zhongyouzk.top

esac
来源：http://zif.yj20258.top

[R12] for 遍历文件
来源：http://rbc.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://esh.sweek.top

[R13] for 计数循环
来源：http://gzh.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://gox.yuxming.cn

[R14] C 风格 for
来源：http://njj.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iap.yuanzhike.top

[R15] while 逐行读文件
来源：http://jxe.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://alj.birdmap.top

[R16] until 等待条件
来源：http://vop.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://orf.cheryme.top

[R17] 数组定义与取值
来源：http://tgq.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://phc.jiagoushi.top

[R18] 遍历数组
来源：http://ftx.xinyue.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hvu.xinyue.icu

[R19] 数组长度
来源：http://lhn.svipenyu.cn

echo "${#arr[@]}"
来源：http://pet.yuanzhike.top

[R20] 关联数组（字典）
来源：http://tnl.zhijiandao.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://syy.jqgufenzy.top

[R21] 字符串长度
来源：http://yip.xingfuxueyuan.xyz

echo "${#s}"
来源：http://xck.cqqwz.cn

[R22] 截取子串
来源：http://enf.ehwqpu.com

echo "${s:0:5}"
来源：http://kkw.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://iln.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rdx.zycfv.cn

[R24] 大小写转换
来源：http://dzp.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://eds.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://cbx.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mex.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://dac.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://dop.hesvh.cn

[R27] 算术展开
来源：http://xkt.yj20258888.top

echo $((1 + 2 * 3))
来源：http://oor.jinghuilouyu.cn

[R28] 浮点运算
来源：http://awf.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://pwe.gaohongyu789.top

[R29] 定义函数
来源：http://hnc.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://unr.tianlin.xyz

[R30] 函数返回状态码
来源：http://pnt.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://xmy.bjfxy.top

[R31] 局部变量
来源：http://wsd.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://ixa.ehwqpu.com

[R32] 参数个数校验
来源：http://sgb.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mqf.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://vdy.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://irb.cqqwz.cn

[R34] 退出时清理
来源：http://gyu.aizwys.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lpb.zdqjudy.top

[R35] 后台执行并等待
来源：http://win.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mch.mhx1999.top

[R36] 并发执行多个任务
来源：http://ero.gzhubu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pfz.52xcode.cn

[R37] 把输出赋给变量
来源：http://xkd.hammf.cn

files=$(ls -1)
来源：http://sxq.zhixingplan.top

[R38] 管道串联
来源：http://oil.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://mql.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://tmc.andypj.xyz

cmd > out.log 2>&1
来源：http://zjx.yonumen.top

[R40] 追加写日志
来源：http://dkf.vqdsnc.cn

echo "log" >> out.log
来源：http://wae.wangshuangyany.cn

[R41] 丢弃输出
来源：http://dzs.xinyue.icu

cmd >/dev/null 2>&1
来源：http://dmy.vqdsnc.cn

[R42] 输入重定向
来源：http://iiv.cheryme.top

wc -l < a.txt
来源：http://cmx.yonumen.top

[R43] 按名字查找文件
来源：http://lai.daxiang520.top

find . -name "*.log" -type f
来源：http://cqu.yonumen.top

[R44] 按修改时间查找
来源：http://tdk.chenlongwang.top

find . -mtime -7 -type f
来源：http://ikr.zycfv.cn

[R45] 批量删除
来源：http://ubb.tarul.cn

find . -name "*.tmp" -delete
来源：http://sve.hesvh.cn

[R46] 递归替换文件内容
来源：http://ywy.tian-w.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gaa.bjfxy.top

[R47] sed 单行替换
来源：http://tzp.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://fnm.ydzc1.top

[R48] awk 取指定列
来源：http://dgt.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://rcw.hnqzz.top

[R49] awk 带条件
来源：http://doa.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ypn.guowangkeji.top

[R50] awk 求和
来源：http://fum.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yow.xziqi.cn

[R51] 排序去重取前几
来源：http://poe.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kbo.yuanzhike.top

[R52] 统计行数
来源：http://cze.hnqzz.top

wc -l a.txt
来源：http://ucb.cheryme.top

[R53] 查看文件头与实时尾
来源：http://tzy.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ebj.zhijiandao.cn

[R54] 比较两个文件
来源：http://ucf.zhixingplan.top

diff a.txt b.txt
来源：http://jsw.pycfn.com

[R55] 压缩与解压
来源：http://fgp.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qfq.zhiwuduotai.top

[R56] 远程拷贝
来源：http://eza.chenzaomai.com

scp file user@host:/path/
来源：http://dne.cucudq.cn

[R57] 远程执行命令
来源：http://wla.cdnleiting.top

ssh user@host 'uptime'
来源：http://vtb.9152youxi.cn

[R58] 下载文件
来源：http://kki.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gby.sxryk.cn

[R59] 发 POST JSON
来源：http://mqz.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://owb.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://rnl.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vrv.shuidangran.top

[R61] 磁盘占用
来源：http://fsi.yj202588.top

df -h;  du -sh *
来源：http://ksx.yvedp.cn

[R62] 找最占空间的文件
来源：http://zgx.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://qxb.nanxinkj.top

[R63] 内存与进程
来源：http://lgv.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://eid.gaohongyu789.top

[R64] 结束进程
来源：http://cgi.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://xkz.fengsongda.top

[R65] 查看端口占用
来源：http://www.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cra.zycfv.cn

[R66] 定时任务
来源：http://kxg.cheryme.top

crontab -e;  crontab -l
来源：http://wpw.hesvh.cn

[R67] 生成随机十六进制串
来源：http://ahk.hcnkem.com

openssl rand -hex 16
来源：http://ejc.xinyue.icu

[R68] 计算文件校验值
来源：http://nki.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://aen.ywan-chungtsiang.top

[R69] 生成随机密码
来源：http://voy.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://hbr.daxiang520.top

[R70] 时间戳与互转
来源：http://ivm.ydzc1.top

date +%s;  date -d @1700000000
来源：http://nca.hesvh.cn

[R71] 日期格式化
来源：http://pzr.havefunace.top


<!-- 参考信息 -->