代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://htf.fengsongda.top

[Q24] 去重
来源：http://kqe.c1oappe.top

SELECT DISTINCT city FROM users;
来源：http://gvo.nwbrower.top

[Q25] 只取前 N 条
来源：http://pic.tarul.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nij.zycfv.cn

[Q26] 计数
来源：http://wav.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://yrm.vehdjk.com

[Q27] 条件计数
来源：http://pih.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://smy.jqgfzy.top

[Q28] 求和与平均
来源：http://szn.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vci.uphjek.com

[Q29] 最大最小值
来源：http://bze.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ypg.daxiang520.top

[Q30] 分组统计
来源：http://ark.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ikj.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://lmt.yj202588.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mht.epnwcf.com

[Q32] 分组拼接字符串
来源：http://cwt.0kj1m.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yhc.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cxo.ivvv.top

[Q33] 多列分组
来源：http://ppz.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iku.tian-w.cn

[Q34] 每组取第一条
来源：http://rmf.hywenlv.cn

SELECT * FROM (
来源：http://xtg.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mio.jiagoushi.top

) t WHERE rn = 1;
来源：http://mbh.yuanzhike.top

[Q35] 内连接
来源：http://fly.kuanghao11.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qvp.xziqi.cn

[Q36] 左连接
来源：http://qky.xuanzx.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ybx.xylfe.cn

[Q37] 右连接
来源：http://tvm.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xpz.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://jws.hnqzz.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tzo.jyoumei.cn

[Q39] 自连接（查上下级）
来源：http://nal.xingfuxueyuan.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://nnp.jlsjyb.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xyr.xuanzx.com

[Q40] 交叉连接（笛卡尔积）
来源：http://dnj.zhongyouzk.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dwr.ydjk.org.cn

[Q41] 多表连接
来源：http://sax.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://bkd.svipenyu.cn

JOIN users u ON u.id = o.user_id
来源：http://qau.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://ghw.yuxming.cn

[Q42] 连接条件附加过滤
来源：http://vcq.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://ukn.zhiwuduotai.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ooz.pycfn.com

[Q43] 标量子查询
来源：http://szf.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ijw.gaohongyu789.top

[Q44] IN 子查询
来源：http://xkn.yuanzhike.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wjq.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://ifw.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://enc.fktsv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wgy.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://itc.cheryme.top

[Q47] 与平均值比较
来源：http://ble.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://toh.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://hok.birdmap.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tzx.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://fbu.ydzc1.top

[Q49] 更新单行
来源：http://umi.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kzv.bjfxy.top

[Q50] 批量更新
来源：http://ijb.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wox.jlsjyb.cn

[Q51] 用子查询更新
来源：http://wgf.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sln.ywan-chungtsiang.top

[Q52] 删除指定行
来源：http://lij.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://nej.ehwqpu.com

[Q53] 按条件删除
来源：http://dtr.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ooi.andypj.xyz

[Q54] 清空表
来源：http://rdk.dashuyun.cn

TRUNCATE TABLE logs;
来源：http://bgl.jinyuanbaomall.cn

[Q55] 排名（并列占位）
来源：http://lms.sufxvd.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vsh.meibo888.top

[Q56] 密集排名（并列不占位）
来源：http://rou.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ncq.shangyingyoupin.top

[Q57] 行号
来源：http://sdl.jqgufenzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rgy.0kj1m.cn

[Q58] 累计求和
来源：http://yon.jinyuanbaomall.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rnz.hesvh.cn

[Q59] 分组内累计
来源：http://cxn.sjlbkw.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kry.sxryk.cn

[Q60] 取上一行 / 下一行
来源：http://scu.cucudq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hwr.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jew.chenzaomai.com

[Q61] 移动平均
来源：http://lsm.jinqigfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nyx.jinyuanbaomall.cn

[Q62] 分组占比
来源：http://abr.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sqf.xuanzx.com

[Q63] 开启事务
来源：http://bhu.ehwqpu.com

START TRANSACTION;                -- 或 BEGIN
来源：http://fts.fzhhl.top

[Q64] 提交事务
来源：http://zoz.kuanghao11.cn

COMMIT;
来源：http://blj.nanxinkj.top

[Q65] 回滚事务
来源：http://dkr.shuidangran.top

ROLLBACK;
来源：http://npf.aizwys.cn

[Q66] 行锁查询
来源：http://ydb.gotoacloud.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ikk.cqqwz.cn

[Q67] 设置隔离级别
来源：http://bxk.hcnkem.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zqb.tianlin.xyz

[Q68] 保存点
来源：http://wzk.xziqi.cn

SAVEPOINT sp1;
来源：http://ean.c1oappe.top

ROLLBACK TO sp1;
来源：http://brw.yonumen.top

[Q69] 查看执行计划
来源：http://bne.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hgi.uphjek.com

[Q70] 更新统计信息
来源：http://pap.cqqwz.cn

ANALYZE TABLE users;
来源：http://xzc.cucudq.cn

[Q71] 查看建表语句
来源：http://xff.gzhubu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kjd.redwolf501.top

[Q72] 查看索引
来源：http://jqd.sxryk.cn

SHOW INDEX FROM users;
来源：http://sfk.uphjek.com

[Q73] 查看表状态
来源：http://qvi.hesvh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uko.birdmap.top

[Q74] 强制使用索引
来源：http://ivw.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eyr.nanxinkj.top

[Q75] 日期格式化
来源：http://afx.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eyx.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jgp.ydjk.org.cn

[Q76] 按天统计
来源：http://mir.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://why.cqqwz.cn

[Q77] 时间加减
来源：http://yjk.xziqi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qvd.svipenyu.cn

[Q78] 当前时间
来源：http://wet.ivvv.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gcj.birdmap.top

[Q79] 字符串拼接
来源：http://okl.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uzi.quarkkingdee.top

[Q80] 字符串截取
来源：http://xua.zhijiandao.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fxh.havefunace.top

[Q81] 字符串替换
来源：http://dtw.hfpthk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wxc.ydzc1.top

[Q82] 字符长度与字节长度
来源：http://kyb.vqdsnc.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://swt.ydzc1.top

[Q83] 大小写转换
来源：http://vhz.xuanzx.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ufj.aizwys.cn

[Q84] 去除首尾空格
来源：http://hsp.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://bti.vehdjk.com

[Q85] 数值取整
来源：http://jsn.chenlongwang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fup.zhijiandao.cn

[Q86] 读取 JSON 字段
来源：http://nyc.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://axp.vehdjk.com

[Q87] JSON 字段做条件
来源：http://rjd.52xcode.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fpp.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://vhj.52xcode.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nli.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bcv.hywenlv.cn

[Q89] 判断表是否存在
来源：http://rcf.ppjwa.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ppz.zhoulong.xyz

[Q90] 生成序号列
来源：http://onq.ydzc1.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pin.jlsjyb.cn

================================================================================
来源：http://bsz.tian-w.cn

R. Bash 专题
来源：http://cvy.hfpthk.cn

================================================================================
来源：http://ngf.bjfxy.top

[R01] shebang 与严格模式
来源：http://uwe.haohaochexian.top

#!/usr/bin/env bash
来源：http://zvw.jinyuanbaomall.cn

set -euo pipefail
来源：http://avh.yvedp.cn

[R02] 变量赋值与使用
来源：http://qrw.cheryme.top

name="Tom"; echo "$name"
来源：http://oar.jinqigfzy.top

[R03] 只读变量
来源：http://jwx.dashuyun.cn

readonly PI=3.14
来源：http://vkh.jqgufenzy.top

[R04] 位置参数
来源：http://clc.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jti.xuetiantiany.cn

[R05] 参数默认值
来源：http://tja.xinyue.icu

name="${1:-default}"
来源：http://gol.haohaochexian.top

[R06] 判断命令是否存在
来源：http://wll.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://enr.zhengqikj.top

[R07] if 判断文件
来源：http://jmo.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xwj.tanke756.top

[R08] 数值比较
来源：http://oks.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://utz.zhoulong.xyz

[R09] 字符串比较
来源：http://flr.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ymf.yonumen.top

[R10] 正则匹配
来源：http://mfd.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zls.andypj.xyz

[R11] case 多分支
来源：http://ktj.yuxming.cn

case "$1" in
来源：http://mgc.iojbl.cn

start) echo "启动" ;;
来源：http://ssj.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://crq.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://yxb.yvedp.cn

esac
来源：http://stx.yueranfly.top

[R12] for 遍历文件
来源：http://kyo.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://hez.nanxuanxn.top

[R13] for 计数循环
来源：http://aap.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://ejs.mhx1999.top

[R14] C 风格 for
来源：http://jvo.yuanzhike.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rel.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://zmp.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zlh.zhixingplan.top

[R16] until 等待条件
来源：http://xoo.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gmo.ehwqpu.com

[R17] 数组定义与取值
来源：http://kqp.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://gua.yangfankeji.com

[R18] 遍历数组
来源：http://jfe.cashguo.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ouf.redwolf501.top

[R19] 数组长度
来源：http://jwr.yj20258888.top

echo "${#arr[@]}"
来源：http://sds.mhx1999.top

[R20] 关联数组（字典）
来源：http://ysi.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rpo.sufxvd.cn

[R21] 字符串长度
来源：http://mkc.fzhhl.top

echo "${#s}"
来源：http://cdc.ivvv.top

[R22] 截取子串
来源：http://tgs.xuetiantiany.cn

echo "${s:0:5}"
来源：http://dlu.yanxiufei.cn

[R23] 字符串替换
来源：http://reo.jlsjyb.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fmz.c1oappe.top

[R24] 大小写转换
来源：http://klo.jinqigufen.top

echo "${s^^}"; echo "${s,,}"
来源：http://ksf.fanxiaobao.xyz

[R25] 去后缀 / 去前缀
来源：http://oyl.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xxz.hongshengwenyu.top

[R26] 命令替换
来源：http://jvy.meibo888.top

now=$(date +%F); echo "$now"
来源：http://fpv.hnxiangtu.top

[R27] 算术展开
来源：http://hvh.yonumen.top

echo $((1 + 2 * 3))
来源：http://qcq.ydzc1.top

[R28] 浮点运算
来源：http://vcz.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://adv.jiagoushi.top

[R29] 定义函数
来源：http://lib.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://btg.316326.xyz

[R30] 函数返回状态码
来源：http://tho.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://nyq.yangfankeji.com

[R31] 局部变量
来源：http://opy.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://eyr.ctjpmb.com

[R32] 参数个数校验
来源：http://ejg.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sav.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://tgl.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://psf.shanyushiyangtech.top

[R34] 退出时清理
来源：http://evy.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://vjl.hnqzz.top

[R35] 后台执行并等待
来源：http://wob.shanyushiyangtech.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cpt.snrcjt.cn

[R36] 并发执行多个任务
来源：http://esk.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://olu.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://gqu.52xcode.cn

files=$(ls -1)
来源：http://xdr.snrcjt.cn

[R38] 管道串联
来源：http://zag.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://vcp.yj20258.top

[R39] 重定向标准输出与错误
来源：http://qdj.smart0.xyz

cmd > out.log 2>&1
来源：http://zrd.redwolf501.top

[R40] 追加写日志
来源：http://cya.sweek.top

echo "log" >> out.log
来源：http://lcc.cashguo.top

[R41] 丢弃输出
来源：http://kdk.guannengcc.top

cmd >/dev/null 2>&1
来源：http://xam.guowangkeji.top

[R42] 输入重定向
来源：http://cem.zhiwuduotai.top

wc -l < a.txt
来源：http://euo.yj202588.top

[R43] 按名字查找文件
来源：http://udg.ydzc1.top

find . -name "*.log" -type f
来源：http://rbu.jlsjyb.cn

[R44] 按修改时间查找
来源：http://tov.gaohongyu789.top

find . -mtime -7 -type f
来源：http://anl.pengpengdd.cyou

[R45] 批量删除
来源：http://cfq.kuanghao11.cn

find . -name "*.tmp" -delete
来源：http://mak.cheryme.top

[R46] 递归替换文件内容
来源：http://tyq.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ebp.gogol.net.cn

[R47] sed 单行替换
来源：http://wve.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://oie.gogol.net.cn

[R48] awk 取指定列
来源：http://kgi.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://tbg.tarul.cn

[R49] awk 带条件
来源：http://uei.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hwx.gogol.net.cn

[R50] awk 求和
来源：http://hbi.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://itn.sxryk.cn

[R51] 排序去重取前几
来源：http://opc.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://zkd.0kj1m.cn

[R52] 统计行数
来源：http://vct.yongpay.top

wc -l a.txt
来源：http://nvb.uphjek.com

[R53] 查看文件头与实时尾
来源：http://bay.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lbx.jyoumei.cn

[R54] 比较两个文件
来源：http://pjx.jianghu66.top

diff a.txt b.txt
来源：http://qem.jlsjyb.cn

[R55] 压缩与解压
来源：http://dfw.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qak.c1oappe.top

[R56] 远程拷贝
来源：http://aou.yfazqb.com

scp file user@host:/path/
来源：http://qqr.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://cal.yvedp.cn

ssh user@host 'uptime'
来源：http://pdv.hfpthk.cn

[R58] 下载文件
来源：http://npq.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tih.aibaodan.cn

[R59] 发 POST JSON
来源：http://hxk.hysaishi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aej.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://zwg.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yrq.316326.xyz

[R61] 磁盘占用
来源：http://acn.nanxuanxn.top

df -h;  du -sh *
来源：http://lhz.hywenlv.cn

[R62] 找最占空间的文件
来源：http://btq.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://mxz.tianlin.xyz

[R63] 内存与进程
来源：http://vga.ivvv.top

free -h;  ps aux | grep nginx
来源：http://ubp.zdbjq.cn

[R64] 结束进程
来源：http://hxj.tianlin.xyz

kill -9 $(pgrep -f app.py)
来源：http://wjr.chenzaomai.com

[R65] 查看端口占用
来源：http://bps.xingfuxueyuan.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vsq.birdmap.top

[R66] 定时任务
来源：http://cgu.nanxinkj.top

crontab -e;  crontab -l
来源：http://hed.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://rex.jinghuilouyu.cn

openssl rand -hex 16
来源：http://kej.yuanzhike.top

[R68] 计算文件校验值
来源：http://afd.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zng.ppjwa.cn

[R69] 生成随机密码
来源：http://hba.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://mrw.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://jus.guannengcc.top

date +%s;  date -d @1700000000
来源：http://lrm.xuetiantiany.cn

[R71] 日期格式化
来源：http://ldb.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mtb.bjfxy.top

[R72] 等待端口就绪
来源：http://cjx.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mps.xingfuxueyuan.xyz

[R73] 分割大日志
来源：http://tiz.yuanzhike.top


<!-- 参考信息 -->