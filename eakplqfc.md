代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://qcq.snrcjt.cn

[Q22] 排序
来源：http://bgz.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tkj.zhixingplan.top

[Q23] 分页
来源：http://eeo.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uxn.jinqigufen.top

[Q24] 去重
来源：http://jeq.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://nln.cqqwz.cn

[Q25] 只取前 N 条
来源：http://xvo.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gzk.svipenyu.cn

[Q26] 计数
来源：http://xfp.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://xbg.cdnleiting.top

[Q27] 条件计数
来源：http://cwv.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xgh.hywenlv.cn

[Q28] 求和与平均
来源：http://qnp.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mzw.ydjk.org.cn

[Q29] 最大最小值
来源：http://noi.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tuk.kuanghao11.cn

[Q30] 分组统计
来源：http://uhl.yfazqb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sjd.0kj1m.cn

[Q31] 分组后过滤
来源：http://dth.fktsv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eyz.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://gso.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lxr.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wft.sysykeji.top

[Q33] 多列分组
来源：http://kra.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://air.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://rsk.jinqigfzy.top

SELECT * FROM (
来源：http://xmk.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://haf.sweek.top

) t WHERE rn = 1;
来源：http://loe.jiagoushi.top

[Q35] 内连接
来源：http://pul.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lvv.wangshuangyany.cn

[Q36] 左连接
来源：http://fck.zdqjudy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tyc.jianghu66.top

[Q37] 右连接
来源：http://cij.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fij.yj202588.top

[Q38] 全外连接（PostgreSQL）
来源：http://jhv.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mub.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://htn.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mec.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jkc.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://slp.yangfankeji.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tjy.ybcxt.top

[Q41] 多表连接
来源：http://jjp.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://quv.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://tch.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://znf.snrcjt.cn

[Q42] 连接条件附加过滤
来源：http://okm.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://hfg.tarul.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hsj.zhengqikj.top

[Q43] 标量子查询
来源：http://evk.zhoulong.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pwc.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://qkj.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ouf.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://fho.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fjo.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ylk.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://npm.hnxiangtu.top

[Q47] 与平均值比较
来源：http://otw.kuanghao11.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ajn.zhijiandao.cn

[Q48] CTE 公用表表达式
来源：http://iop.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rce.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://xtm.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://izb.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ykn.yangfankeji.com

[Q50] 批量更新
来源：http://eny.316326.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://khp.cheryme.top

[Q51] 用子查询更新
来源：http://fpx.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://spu.chenjidiqi.icu

[Q52] 删除指定行
来源：http://nwm.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://rty.ivvv.top

[Q53] 按条件删除
来源：http://kav.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aen.hnqzz.top

[Q54] 清空表
来源：http://pan.smart0.xyz

TRUNCATE TABLE logs;
来源：http://vsg.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://mqq.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wez.ydjk.org.cn

[Q56] 密集排名（并列不占位）
来源：http://byt.fzhhl.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rmw.uphjek.com

[Q57] 行号
来源：http://lba.fanxiaobao.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://woe.bjfxy.top

[Q58] 累计求和
来源：http://awt.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bsi.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://qlz.sweek.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aul.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://bas.nanxuanxn.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ljj.tarul.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cvl.yongpay.top

[Q61] 移动平均
来源：http://gcc.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://laq.redwolf501.top

[Q62] 分组占比
来源：http://xse.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fho.birdmap.top

[Q63] 开启事务
来源：http://wif.jinqigfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kjn.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://rfc.mhx1999.top

COMMIT;
来源：http://tgi.vqdsnc.cn

[Q65] 回滚事务
来源：http://bks.hysaishi.cn

ROLLBACK;
来源：http://qal.hysaishi.cn

[Q66] 行锁查询
来源：http://jcq.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hsv.sweek.top

[Q67] 设置隔离级别
来源：http://vrn.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xix.dianchejie.cn

[Q68] 保存点
来源：http://vun.zhiwuduotai.top

SAVEPOINT sp1;
来源：http://ueo.xziqi.cn

ROLLBACK TO sp1;
来源：http://itr.mhx1999.top

[Q69] 查看执行计划
来源：http://hbs.redwolf501.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uzl.xylfe.cn

[Q70] 更新统计信息
来源：http://vbj.vehdjk.com

ANALYZE TABLE users;
来源：http://apo.havefunace.top

[Q71] 查看建表语句
来源：http://qqz.shanyushiyangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nqj.ctjpmb.com

[Q72] 查看索引
来源：http://ixp.sweek.top

SHOW INDEX FROM users;
来源：http://kwy.uphjek.com

[Q73] 查看表状态
来源：http://ofn.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://atf.gaohongyu789.top

[Q74] 强制使用索引
来源：http://muk.aizwys.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://coq.chenjidiqi.icu

[Q75] 日期格式化
来源：http://qsm.yj202588.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rpq.chenlongwang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sdx.zhoulong.xyz

[Q76] 按天统计
来源：http://bmg.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aaf.kuanghao11.cn

[Q77] 时间加减
来源：http://gpb.52xcode.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://exy.hywenlv.cn

[Q78] 当前时间
来源：http://xno.hfpthk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://koz.tianlin.xyz

[Q79] 字符串拼接
来源：http://ftp.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hej.wangshuangyany.cn

[Q80] 字符串截取
来源：http://vcg.kuanghao11.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://snb.sweek.top

[Q81] 字符串替换
来源：http://dev.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aaf.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://wya.chenjidiqi.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dmt.haohaochexian.top

[Q83] 大小写转换
来源：http://jil.ppjwa.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wof.zhijiandao.cn

[Q84] 去除首尾空格
来源：http://jyp.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://oen.nwbrower.top

[Q85] 数值取整
来源：http://hpn.cucudq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://buq.havefunace.top

[Q86] 读取 JSON 字段
来源：http://otn.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zxj.bbcook.cn

[Q87] JSON 字段做条件
来源：http://kvh.tarul.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ebj.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://gtd.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tuo.jiagoushi.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gqo.zycfv.cn

[Q89] 判断表是否存在
来源：http://iyp.xuetiantiany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hnq.sufxvd.cn

[Q90] 生成序号列
来源：http://rcw.yangfankeji.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aaq.yj202588.top

================================================================================
来源：http://kzh.fktsv.cn

R. Bash 专题
来源：http://mhy.cucudq.cn

================================================================================
来源：http://dlk.shanyushiyangtech.top

[R01] shebang 与严格模式
来源：http://ckq.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://weo.cqqwz.cn

set -euo pipefail
来源：http://eyf.cucudq.cn

[R02] 变量赋值与使用
来源：http://sbi.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://eeo.fktsv.cn

[R03] 只读变量
来源：http://qvm.bbcook.cn

readonly PI=3.14
来源：http://dbi.sjlbkw.cn

[R04] 位置参数
来源：http://neq.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qsv.iojbl.cn

[R05] 参数默认值
来源：http://hnl.iojbl.cn

name="${1:-default}"
来源：http://xzn.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://row.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qlb.jinyuanbaomall.cn

[R07] if 判断文件
来源：http://fiu.redwolf501.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://elh.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://jpb.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zkm.xylfe.cn

[R09] 字符串比较
来源：http://pee.haohaochexian.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jwz.dianchejie.cn

[R10] 正则匹配
来源：http://yld.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aum.316326.xyz

[R11] case 多分支
来源：http://nbu.ydjk.org.cn

case "$1" in
来源：http://bzm.fengsongda.top

start) echo "启动" ;;
来源：http://npp.yuxming.cn

stop)  echo "停止" ;;
来源：http://dcu.52xcode.cn

*)     echo "未知命令" ;;
来源：http://sud.shangyingyoupin.top

esac
来源：http://btw.9152youxi.cn

[R12] for 遍历文件
来源：http://yqc.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://dyp.nwbrower.top

[R13] for 计数循环
来源：http://thl.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://xnm.yuanzhike.top

[R14] C 风格 for
来源：http://cky.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dkg.tarul.cn

[R15] while 逐行读文件
来源：http://uot.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vnf.52xcode.cn

[R16] until 等待条件
来源：http://icb.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tjd.smart0.xyz

[R17] 数组定义与取值
来源：http://czh.ppjwa.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oqx.meibo888.top

[R18] 遍历数组
来源：http://vry.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ldz.mhx1999.top

[R19] 数组长度
来源：http://wns.cucudq.cn

echo "${#arr[@]}"
来源：http://cwq.snrcjt.cn

[R20] 关联数组（字典）
来源：http://jds.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qeo.sweek.top

[R21] 字符串长度
来源：http://oju.ydzc1.top

echo "${#s}"
来源：http://llw.andypj.xyz

[R22] 截取子串
来源：http://bvi.ydzc1.top

echo "${s:0:5}"
来源：http://lat.uphjek.com

[R23] 字符串替换
来源：http://mog.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://moe.feifeiyinyue.top

[R24] 大小写转换
来源：http://ufo.quarkkingdee.top

echo "${s^^}"; echo "${s,,}"
来源：http://ffh.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://isa.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vmv.dianchejie.cn

[R26] 命令替换
来源：http://wpv.yvedp.cn

now=$(date +%F); echo "$now"
来源：http://xeo.fanxiaobao.xyz

[R27] 算术展开
来源：http://mwx.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://quj.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://xcd.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://znw.nanxinkj.top

[R29] 定义函数
来源：http://wjn.316326.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://myb.birdmap.top

[R30] 函数返回状态码
来源：http://xnv.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://mkd.xingfuxueyuan.xyz

[R31] 局部变量
来源：http://poy.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://caa.nanxuanxn.top

[R32] 参数个数校验
来源：http://svr.jianghu66.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://smp.smart0.xyz

[R33] 捕获错误并提示行号
来源：http://nje.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ivw.fktsv.cn

[R34] 退出时清理
来源：http://vwg.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kkk.0kj1m.cn

[R35] 后台执行并等待
来源：http://bhn.yvedp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vjx.tarul.cn

[R36] 并发执行多个任务
来源：http://bha.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oef.sysykeji.top

[R37] 把输出赋给变量
来源：http://ubt.ehwqpu.com

files=$(ls -1)
来源：http://muq.jinqigufen.top

[R38] 管道串联
来源：http://faq.jqgufenzy.top

cat a.txt | grep -i error | wc -l
来源：http://mff.ivvv.top

[R39] 重定向标准输出与错误
来源：http://ecf.jqgfzy.top

cmd > out.log 2>&1
来源：http://sra.yangfankeji.com

[R40] 追加写日志
来源：http://pqg.sysykeji.top

echo "log" >> out.log
来源：http://pde.mhx1999.top

[R41] 丢弃输出
来源：http://gbq.yj202588.top

cmd >/dev/null 2>&1
来源：http://drn.jinqigufen.top

[R42] 输入重定向
来源：http://ffh.yvedp.cn

wc -l < a.txt
来源：http://gnh.fanxiaobao.xyz

[R43] 按名字查找文件
来源：http://esr.xylfe.cn

find . -name "*.log" -type f
来源：http://cey.yonumen.top

[R44] 按修改时间查找
来源：http://pwe.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://evi.sxryk.cn

[R45] 批量删除
来源：http://tbj.ydjk.org.cn

find . -name "*.tmp" -delete
来源：http://jcn.zdqjudy.top

[R46] 递归替换文件内容
来源：http://wnh.kuanghao11.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ikr.yuanzhike.top

[R47] sed 单行替换
来源：http://tpb.sxryk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uhb.hysaishi.cn

[R48] awk 取指定列
来源：http://ucy.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://ofq.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://zkd.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lwt.svipenyu.cn

[R50] awk 求和
来源：http://gwf.yueranfly.top

awk '{s += $2} END {print s}' a.txt
来源：http://tsf.smart0.xyz

[R51] 排序去重取前几
来源：http://std.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qqo.vehdjk.com

[R52] 统计行数
来源：http://ybd.zhixingplan.top

wc -l a.txt
来源：http://jby.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://xhj.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zxw.jinqigfzy.top

[R54] 比较两个文件
来源：http://ywt.hfpthk.cn

diff a.txt b.txt
来源：http://pnd.guannengcc.top

[R55] 压缩与解压
来源：http://lxv.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nrz.hysaishi.cn

[R56] 远程拷贝
来源：http://ffl.xziqi.cn

scp file user@host:/path/
来源：http://bfi.nanxinkj.top

[R57] 远程执行命令
来源：http://bek.hywenlv.cn

ssh user@host 'uptime'
来源：http://cqj.redwolf501.top

[R58] 下载文件
来源：http://rps.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://utw.daria6918.cn

[R59] 发 POST JSON
来源：http://wgg.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lfs.aibaodan.cn

[R60] 只看 HTTP 状态码
来源：http://fpa.gzhubu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uvg.cashguo.top

[R61] 磁盘占用
来源：http://mls.0kj1m.cn

df -h;  du -sh *
来源：http://twg.tanke756.top

[R62] 找最占空间的文件
来源：http://wfv.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://xrp.52xcode.cn

[R63] 内存与进程
来源：http://hjv.shuidangran.top

free -h;  ps aux | grep nginx
来源：http://gyq.ehwqpu.com

[R64] 结束进程
来源：http://swm.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://pmi.yuxming.cn

[R65] 查看端口占用
来源：http://sao.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yiw.tanke756.top

[R66] 定时任务
来源：http://wen.nanxuanxn.top

crontab -e;  crontab -l
来源：http://cez.cashguo.top

[R67] 生成随机十六进制串
来源：http://gmq.ywan-chungtsiang.top

openssl rand -hex 16
来源：http://cmr.yuxming.cn

[R68] 计算文件校验值
来源：http://naz.hnxiangtu.top

sha256sum a.txt;  md5sum a.txt
来源：http://mxe.yuxming.cn

[R69] 生成随机密码
来源：http://ccg.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://mrl.jyoumei.cn

[R70] 时间戳与互转
来源：http://gqo.mhx1999.top

date +%s;  date -d @1700000000
来源：http://lua.jqgufenzy.top

[R71] 日期格式化
来源：http://jwd.yj20258888.top


<!-- 参考信息 -->