代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mxx.zhoulong.xyz

[Q20] IN 列表
来源：http://did.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hfg.iojbl.cn

[Q21] 空值判断
来源：http://fbs.shangyingyoupin.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pxz.zdqjudy.top

[Q22] 排序
来源：http://epl.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bao.shangyingyoupin.top

[Q23] 分页
来源：http://mbs.yj20258.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uxk.birdmap.top

[Q24] 去重
来源：http://ouj.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://hbq.chenzaomai.com

[Q25] 只取前 N 条
来源：http://msi.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sln.gaohongyu789.top

[Q26] 计数
来源：http://pqc.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://uzm.52xcode.cn

[Q27] 条件计数
来源：http://nch.shzxlz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://une.xuanzx.com

[Q28] 求和与平均
来源：http://deo.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xoa.sjlbkw.cn

[Q29] 最大最小值
来源：http://chd.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://aqm.ehwqpu.com

[Q30] 分组统计
来源：http://dmz.tarul.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gti.yj20258.top

[Q31] 分组后过滤
来源：http://lnw.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qjd.dashuyun.cn

[Q32] 分组拼接字符串
来源：http://ubj.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qlx.ehwqpu.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vaw.vehdjk.com

[Q33] 多列分组
来源：http://liq.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rsw.havefunace.top

[Q34] 每组取第一条
来源：http://ojc.gogol.net.cn

SELECT * FROM (
来源：http://juc.haohaochexian.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rft.zhijiandao.cn

) t WHERE rn = 1;
来源：http://rrz.gogol.net.cn

[Q35] 内连接
来源：http://tap.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://szz.havefunace.top

[Q36] 左连接
来源：http://exn.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://avy.fzhhl.top

[Q37] 右连接
来源：http://fna.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dzo.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://puu.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hkc.birdmap.top

[Q39] 自连接（查上下级）
来源：http://jsn.iojbl.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ovm.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mqm.cucudq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qwn.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lqv.cqqwz.cn

[Q41] 多表连接
来源：http://bac.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lli.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://kyr.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://lsr.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://gld.yfazqb.com

SELECT u.name, o.amount FROM users u
来源：http://ndg.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vaj.uphjek.com

[Q43] 标量子查询
来源：http://quq.cdnleiting.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jkn.xuetiantiany.cn

[Q44] IN 子查询
来源：http://jlq.yj202588.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xzj.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://iik.yvedp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mdh.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wfz.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://que.jqgfzy.top

[Q47] 与平均值比较
来源：http://tek.wangdashe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mqx.andypj.xyz

[Q48] CTE 公用表表达式
来源：http://rld.hywenlv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://anu.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://akj.havefunace.top

[Q49] 更新单行
来源：http://uck.gotoacloud.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hhb.gzhubu.top

[Q50] 批量更新
来源：http://csy.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gsz.quarkkingdee.top

[Q51] 用子查询更新
来源：http://qoi.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qpj.gogol.net.cn

[Q52] 删除指定行
来源：http://pvg.tian-w.cn

DELETE FROM users WHERE id = 10;
来源：http://rab.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://hcf.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://goc.shanyushiyangkeji.top

[Q54] 清空表
来源：http://uvx.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://kmx.snrcjt.cn

[Q55] 排名（并列占位）
来源：http://cjv.uphjek.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ruc.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://ceq.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://imp.svipenyu.cn

[Q57] 行号
来源：http://dbi.wangshuangyany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dhj.yj20258888.top

[Q58] 累计求和
来源：http://mma.nwbrower.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ahi.wangdashe.top

[Q59] 分组内累计
来源：http://gmd.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://euc.birdmap.top

[Q60] 取上一行 / 下一行
来源：http://use.gaohongyu789.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://grh.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cbk.yongpay.top

[Q61] 移动平均
来源：http://uwc.vqdsnc.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cqx.meibo888.top

[Q62] 分组占比
来源：http://vun.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://auu.cheryme.top

[Q63] 开启事务
来源：http://dgi.uphjek.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ymm.xuanzx.com

[Q64] 提交事务
来源：http://nuj.zdqjudy.top

COMMIT;
来源：http://gzq.zhoulong.xyz

[Q65] 回滚事务
来源：http://vut.chenlongwang.top

ROLLBACK;
来源：http://zaq.hnqzz.top

[Q66] 行锁查询
来源：http://zey.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tlg.yonumen.top

[Q67] 设置隔离级别
来源：http://zzf.havefunace.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tov.vqdsnc.cn

[Q68] 保存点
来源：http://qnc.ywan-chungtsiang.top

SAVEPOINT sp1;
来源：http://alw.uphjek.com

ROLLBACK TO sp1;
来源：http://gnl.nwbrower.top

[Q69] 查看执行计划
来源：http://gxd.gzhubu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mpn.hammf.cn

[Q70] 更新统计信息
来源：http://kcm.gzhubu.top

ANALYZE TABLE users;
来源：http://xxf.zhongyouzk.top

[Q71] 查看建表语句
来源：http://wlj.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uzp.jqgfzy.top

[Q72] 查看索引
来源：http://tst.bbcook.cn

SHOW INDEX FROM users;
来源：http://gxp.yuanzhike.top

[Q73] 查看表状态
来源：http://fzo.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tqj.epnwcf.com

[Q74] 强制使用索引
来源：http://vit.gzhubu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ewm.hongshengwenyu.top

[Q75] 日期格式化
来源：http://dsh.yfazqb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jtr.yonumen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yxm.chenjidiqi.icu

[Q76] 按天统计
来源：http://oby.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eoc.fanxiaobao.xyz

[Q77] 时间加减
来源：http://ngg.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://msx.wangdashe.top

[Q78] 当前时间
来源：http://oxh.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dow.uphjek.com

[Q79] 字符串拼接
来源：http://bqi.snrcjt.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hle.andypj.xyz

[Q80] 字符串截取
来源：http://qpg.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nho.fktsv.cn

[Q81] 字符串替换
来源：http://ekw.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dyd.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://rbu.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qoc.haohaochexian.top

[Q83] 大小写转换
来源：http://wne.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xyx.cashguo.top

[Q84] 去除首尾空格
来源：http://swm.iojbl.cn

SELECT TRIM(name) FROM users;
来源：http://bla.hysaishi.cn

[Q85] 数值取整
来源：http://oly.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yzh.mhx1999.top

[Q86] 读取 JSON 字段
来源：http://ite.shanyushiyangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qfa.sxryk.cn

[Q87] JSON 字段做条件
来源：http://ziz.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ypj.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://upn.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ymb.andypj.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kjd.guannengcc.top

[Q89] 判断表是否存在
来源：http://uoz.zhengqikj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lal.haohaochexian.top

[Q90] 生成序号列
来源：http://mxj.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ugg.zhiwuduotai.top

================================================================================
来源：http://wth.yj20258.top

R. Bash 专题
来源：http://uhj.wangdashe.top

================================================================================
来源：http://cmw.fzhhl.top

[R01] shebang 与严格模式
来源：http://jpq.vqdsnc.cn

#!/usr/bin/env bash
来源：http://tcd.mhx1999.top

set -euo pipefail
来源：http://eou.andypj.xyz

[R02] 变量赋值与使用
来源：http://eah.vqdsnc.cn

name="Tom"; echo "$name"
来源：http://swg.hysaishi.cn

[R03] 只读变量
来源：http://npp.yuanzhike.top

readonly PI=3.14
来源：http://rcr.jinghuilouyu.cn

[R04] 位置参数
来源：http://gtr.yonumen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mxq.yj20258.top

[R05] 参数默认值
来源：http://jkt.cdnleiting.top

name="${1:-default}"
来源：http://zdu.smart0.xyz

[R06] 判断命令是否存在
来源：http://evy.jinqigfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://txt.jinghuilouyu.cn

[R07] if 判断文件
来源：http://iij.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://llb.ydzc1.top

[R08] 数值比较
来源：http://jml.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://lyu.yj202588.top

[R09] 字符串比较
来源：http://eos.bbcook.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bvu.snrcjt.cn

[R10] 正则匹配
来源：http://pnz.zhongyouzk.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://okg.shuidangran.top

[R11] case 多分支
来源：http://wst.dashuyun.cn

case "$1" in
来源：http://pfj.uphjek.com

start) echo "启动" ;;
来源：http://klk.52xcode.cn

stop)  echo "停止" ;;
来源：http://lbv.xuanzx.com

*)     echo "未知命令" ;;
来源：http://lsm.chenlongwang.top

esac
来源：http://syq.dianchejie.cn

[R12] for 遍历文件
来源：http://cpr.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://lnw.chenlongwang.top

[R13] for 计数循环
来源：http://icz.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://zyk.pycfn.com

[R14] C 风格 for
来源：http://yqi.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uyw.daria6918.cn

[R15] while 逐行读文件
来源：http://sto.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pds.hammf.cn

[R16] until 等待条件
来源：http://hku.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fbq.ydzc1.top

[R17] 数组定义与取值
来源：http://zxq.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ood.yj20258.top

[R18] 遍历数组
来源：http://ouf.xziqi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ctr.chenjidiqi.icu

[R19] 数组长度
来源：http://sie.yuxming.cn

echo "${#arr[@]}"
来源：http://efe.52xcode.cn

[R20] 关联数组（字典）
来源：http://qbd.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lua.hywenlv.cn

[R21] 字符串长度
来源：http://xyz.jianghu66.top

echo "${#s}"
来源：http://zbn.hongshengwenyu.top

[R22] 截取子串
来源：http://pmb.nwbrower.top

echo "${s:0:5}"
来源：http://nro.zdbjq.cn

[R23] 字符串替换
来源：http://zpu.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ore.xylfe.cn

[R24] 大小写转换
来源：http://oaj.yangfankeji.com

echo "${s^^}"; echo "${s,,}"
来源：http://bhd.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://gvh.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://bsv.iojbl.cn

[R26] 命令替换
来源：http://fax.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://jjb.nanxinkj.top

[R27] 算术展开
来源：http://yxx.kuanghao11.cn

echo $((1 + 2 * 3))
来源：http://kiw.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://gpb.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://hvv.pycfn.com

[R29] 定义函数
来源：http://fkj.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dcb.andypj.xyz

[R30] 函数返回状态码
来源：http://klu.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://rjt.andypj.xyz

[R31] 局部变量
来源：http://hdk.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://qvx.bbcook.cn

[R32] 参数个数校验
来源：http://enc.tian-w.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nyp.xziqi.cn

[R33] 捕获错误并提示行号
来源：http://jkt.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aiu.yfazqb.com

[R34] 退出时清理
来源：http://ybd.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://jao.tian-w.cn

[R35] 后台执行并等待
来源：http://dfw.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://srq.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://bep.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://biw.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://znu.tianlin.xyz

files=$(ls -1)
来源：http://urw.shzxlz.cn

[R38] 管道串联
来源：http://nwk.fengsongda.top

cat a.txt | grep -i error | wc -l
来源：http://tuw.tanke756.top

[R39] 重定向标准输出与错误
来源：http://owz.yuanzhike.top

cmd > out.log 2>&1
来源：http://qql.ehwqpu.com

[R40] 追加写日志
来源：http://jii.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://dkt.zdbjq.cn

[R41] 丢弃输出
来源：http://lbn.shanyushiyangkeji.top

cmd >/dev/null 2>&1
来源：http://meb.jinyuanbaomall.cn

[R42] 输入重定向
来源：http://vin.zhiwuduotai.top

wc -l < a.txt
来源：http://odw.redwolf501.top

[R43] 按名字查找文件
来源：http://mvh.xuanzx.com

find . -name "*.log" -type f
来源：http://ivp.ydjk.org.cn

[R44] 按修改时间查找
来源：http://ilt.zhijiandao.cn

find . -mtime -7 -type f
来源：http://hmo.zhixingplan.top

[R45] 批量删除
来源：http://shk.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://npb.shanyushiyangtech.top

[R46] 递归替换文件内容
来源：http://qzi.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://prq.gotoacloud.top

[R47] sed 单行替换
来源：http://jqh.fktsv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://klw.52xcode.cn

[R48] awk 取指定列
来源：http://iqy.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://xiy.xuanzx.com

[R49] awk 带条件
来源：http://sxl.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jqx.ydzc1.top

[R50] awk 求和
来源：http://fxu.c1oappe.top

awk '{s += $2} END {print s}' a.txt
来源：http://kru.havefunace.top

[R51] 排序去重取前几
来源：http://iqj.yj202588.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ogn.fanxiaobao.xyz

[R52] 统计行数
来源：http://lhz.hysaishi.cn

wc -l a.txt
来源：http://tce.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://ptr.yuxming.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hjc.tianlin.xyz

[R54] 比较两个文件
来源：http://mxa.feifeiyinyue.top

diff a.txt b.txt
来源：http://ijh.bbcook.cn

[R55] 压缩与解压
来源：http://gza.jqgufenzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pco.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://zwc.tarul.cn

scp file user@host:/path/
来源：http://bps.aibaodan.cn

[R57] 远程执行命令
来源：http://qya.zdbjq.cn

ssh user@host 'uptime'
来源：http://tck.fehbvm.com

[R58] 下载文件
来源：http://fys.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ska.uphjek.com

[R59] 发 POST JSON
来源：http://pfx.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sgn.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://bzw.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xjc.jiagoushi.top

[R61] 磁盘占用
来源：http://ywt.yangfankeji.com

df -h;  du -sh *
来源：http://rqu.jinqigufen.top

[R62] 找最占空间的文件
来源：http://qzb.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://rcz.hesvh.cn

[R63] 内存与进程
来源：http://bup.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://hmm.gaohongyu789.top

[R64] 结束进程
来源：http://ruk.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://cbi.hesvh.cn

[R65] 查看端口占用
来源：http://iiv.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rnn.cheryme.top

[R66] 定时任务
来源：http://hfh.chenzaomai.com

crontab -e;  crontab -l
来源：http://psj.ydjk.org.cn

[R67] 生成随机十六进制串
来源：http://bya.hnqzz.top

openssl rand -hex 16
来源：http://nrc.yonumen.top

[R68] 计算文件校验值
来源：http://lhh.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://klv.chenlongwang.top

[R69] 生成随机密码
来源：http://axu.aizwys.cn


<!-- 参考信息 -->