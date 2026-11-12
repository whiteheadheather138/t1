代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zfs.ctjpmb.com

[Q26] 计数
来源：http://sbt.jinyuanbaomall.cn

SELECT COUNT(*) FROM users;
来源：http://hdu.yongpay.top

[Q27] 条件计数
来源：http://hjf.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hfp.fengsongda.top

[Q28] 求和与平均
来源：http://bsy.hesvh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pmz.ehwqpu.com

[Q29] 最大最小值
来源：http://icn.zhijiandao.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vds.fehbvm.com

[Q30] 分组统计
来源：http://ara.aizwys.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vwq.hywenlv.cn

[Q31] 分组后过滤
来源：http://uje.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hgf.shuidangran.top

[Q32] 分组拼接字符串
来源：http://hya.cashguo.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hfr.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://owa.zhijiandao.cn

[Q33] 多列分组
来源：http://cfa.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tfa.cucudq.cn

[Q34] 每组取第一条
来源：http://bor.shzxlz.cn

SELECT * FROM (
来源：http://pzq.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sep.52xcode.cn

) t WHERE rn = 1;
来源：http://xsg.vqdsnc.cn

[Q35] 内连接
来源：http://aps.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yno.wangshuangyany.cn

[Q36] 左连接
来源：http://ojd.iojbl.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://enu.jqgufenzy.top

[Q37] 右连接
来源：http://plm.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ytn.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://eyd.jinyuanbaomall.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jgr.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://eka.quarkkingdee.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tre.kuanghao11.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qep.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gqz.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eom.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://uia.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ztb.chenjidiqi.icu

JOIN users u ON u.id = o.user_id
来源：http://fgb.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://iif.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://whz.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://por.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iws.guowangkeji.top

[Q43] 标量子查询
来源：http://bfb.hesvh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jyd.ehwqpu.com

[Q44] IN 子查询
来源：http://hzc.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tjp.gaohongyu789.top

[Q45] EXISTS 判断存在
来源：http://pqs.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qhz.sxryk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zyk.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bgp.chenlongwang.top

[Q47] 与平均值比较
来源：http://fgo.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ioy.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://evj.yonumen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kcw.ydzc1.top

SELECT * FROM t WHERE c > 5;
来源：http://gjw.jlsjyb.cn

[Q49] 更新单行
来源：http://baj.shangyingyoupin.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jqx.vqdsnc.cn

[Q50] 批量更新
来源：http://quu.guannengcc.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ubw.yj20258.top

[Q51] 用子查询更新
来源：http://drk.tian-w.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oog.hnxiangtu.top

[Q52] 删除指定行
来源：http://czn.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://ums.yj20258888.top

[Q53] 按条件删除
来源：http://ikt.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://klu.zhixingplan.top

[Q54] 清空表
来源：http://ljr.xuetiantiany.cn

TRUNCATE TABLE logs;
来源：http://nmy.smart0.xyz

[Q55] 排名（并列占位）
来源：http://bqc.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yai.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://nsw.yj202588.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://odx.feifeiyinyue.top

[Q57] 行号
来源：http://ckb.yj20258.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ksu.dashuyun.cn

[Q58] 累计求和
来源：http://kep.hammf.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ukb.daxiang520.top

[Q59] 分组内累计
来源：http://noh.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mqp.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://rha.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sle.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fhu.jqgfzy.top

[Q61] 移动平均
来源：http://cwb.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hsv.c1oappe.top

[Q62] 分组占比
来源：http://mqu.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ojq.sxryk.cn

[Q63] 开启事务
来源：http://wmv.quarkkingdee.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pdl.yj20258.top

[Q64] 提交事务
来源：http://yyf.cheryme.top

COMMIT;
来源：http://nhd.ydjk.org.cn

[Q65] 回滚事务
来源：http://pxm.zhiwuduotai.top

ROLLBACK;
来源：http://xnw.jinqigfzy.top

[Q66] 行锁查询
来源：http://efg.xingfuxueyuan.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cfl.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://hpm.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kxp.gotoacloud.top

[Q68] 保存点
来源：http://vph.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://wyw.hongshengwenyu.top

ROLLBACK TO sp1;
来源：http://zzh.meibo888.top

[Q69] 查看执行计划
来源：http://mwh.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://egi.hnqzz.top

[Q70] 更新统计信息
来源：http://lxw.ydjk.org.cn

ANALYZE TABLE users;
来源：http://mlu.xziqi.cn

[Q71] 查看建表语句
来源：http://sxu.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ypr.aizwys.cn

[Q72] 查看索引
来源：http://uin.sweek.top

SHOW INDEX FROM users;
来源：http://abg.cucudq.cn

[Q73] 查看表状态
来源：http://aru.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vyk.chenlongwang.top

[Q74] 强制使用索引
来源：http://nls.xingfuxueyuan.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://acb.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://gne.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qgr.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ubr.yanxiufei.cn

[Q76] 按天统计
来源：http://bld.jinghuilouyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ojz.ehwqpu.com

[Q77] 时间加减
来源：http://ads.chenjidiqi.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qzy.pengpengdd.cyou

[Q78] 当前时间
来源：http://rgj.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ysy.yvedp.cn

[Q79] 字符串拼接
来源：http://nvu.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vwo.xuanzx.com

[Q80] 字符串截取
来源：http://mha.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eif.iojbl.cn

[Q81] 字符串替换
来源：http://sat.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ggn.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://pyc.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zvq.zhijiandao.cn

[Q83] 大小写转换
来源：http://xbv.xuanzx.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jps.uphjek.com

[Q84] 去除首尾空格
来源：http://vvu.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://uxn.sweek.top

[Q85] 数值取整
来源：http://shy.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qnt.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://ram.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qwv.bjfxy.top

[Q87] JSON 字段做条件
来源：http://wdl.zhixingplan.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yqj.birdmap.top

[Q88] 行转列（条件聚合）
来源：http://vxf.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jij.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xie.yangfankeji.com

[Q89] 判断表是否存在
来源：http://fgq.sxryk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://szr.meibo888.top

[Q90] 生成序号列
来源：http://gnq.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qlo.jianghu66.top

================================================================================
来源：http://jzk.ctjpmb.com

R. Bash 专题
来源：http://oey.mhx1999.top

================================================================================
来源：http://ohf.bjfxy.top

[R01] shebang 与严格模式
来源：http://wld.fzhhl.top

#!/usr/bin/env bash
来源：http://sdt.zhiwuduotai.top

set -euo pipefail
来源：http://lhk.vehdjk.com

[R02] 变量赋值与使用
来源：http://dqc.hcnkem.com

name="Tom"; echo "$name"
来源：http://djq.meibo888.top

[R03] 只读变量
来源：http://jya.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://cid.jinqigufen.top

[R04] 位置参数
来源：http://byt.nwbrower.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pbe.zdbjq.cn

[R05] 参数默认值
来源：http://acn.gzhubu.top

name="${1:-default}"
来源：http://gbs.xylfe.cn

[R06] 判断命令是否存在
来源：http://lyz.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hre.aizwys.cn

[R07] if 判断文件
来源：http://ikk.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sgh.nanxuanxn.top

[R08] 数值比较
来源：http://cxi.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://lou.yuxming.cn

[R09] 字符串比较
来源：http://gdl.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uxj.jyoumei.cn

[R10] 正则匹配
来源：http://woe.daria6918.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://alt.fehbvm.com

[R11] case 多分支
来源：http://qrf.jyoumei.cn

case "$1" in
来源：http://tvk.xingfuxueyuan.xyz

start) echo "启动" ;;
来源：http://egm.daria6918.cn

stop)  echo "停止" ;;
来源：http://own.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://ecg.tian-w.cn

esac
来源：http://wge.bbcook.cn

[R12] for 遍历文件
来源：http://wbq.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://ptc.ydjk.org.cn

[R13] for 计数循环
来源：http://nim.jinyuanbaomall.cn

for i in {1..10}; do echo "$i"; done
来源：http://ewi.0kj1m.cn

[R14] C 风格 for
来源：http://nlf.yanxiufei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ipn.epnwcf.com

[R15] while 逐行读文件
来源：http://xrd.redwolf501.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bgm.zdqjudy.top

[R16] until 等待条件
来源：http://rev.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://boc.zycfv.cn

[R17] 数组定义与取值
来源：http://raa.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://fpi.quarkkingdee.top

[R18] 遍历数组
来源：http://pvw.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kmb.xylfe.cn

[R19] 数组长度
来源：http://tuu.pycfn.com

echo "${#arr[@]}"
来源：http://mkh.havefunace.top

[R20] 关联数组（字典）
来源：http://nhg.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ihf.nanxinkj.top

[R21] 字符串长度
来源：http://ino.sjlbkw.cn

echo "${#s}"
来源：http://hmc.aizwys.cn

[R22] 截取子串
来源：http://vvz.daria6918.cn

echo "${s:0:5}"
来源：http://gjv.ppjwa.cn

[R23] 字符串替换
来源：http://yvc.hammf.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xmh.hnqzz.top

[R24] 大小写转换
来源：http://iro.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://hwp.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://nsj.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://txc.nanxuanxn.top

[R26] 命令替换
来源：http://fod.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://yev.0kj1m.cn

[R27] 算术展开
来源：http://kzc.xylfe.cn

echo $((1 + 2 * 3))
来源：http://jeq.yj202588.top

[R28] 浮点运算
来源：http://enm.sufxvd.cn

echo "scale=2; 10/3" | bc
来源：http://wrh.birdmap.top

[R29] 定义函数
来源：http://beq.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zih.gzhubu.top

[R30] 函数返回状态码
来源：http://yry.xingfuxueyuan.xyz

f() { return 0; }; f || echo "失败了"
来源：http://kjj.birdmap.top

[R31] 局部变量
来源：http://tcs.xylfe.cn

f() { local x=1; echo "$x"; }
来源：http://wdf.0kj1m.cn

[R32] 参数个数校验
来源：http://qzg.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jwc.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://qmm.nanxuanxn.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wey.cheryme.top

[R34] 退出时清理
来源：http://afm.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://tlq.guannengcc.top

[R35] 后台执行并等待
来源：http://azh.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wqe.yueranfly.top

[R36] 并发执行多个任务
来源：http://hkr.cqqwz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://epc.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://rlp.cashguo.top

files=$(ls -1)
来源：http://yrq.iojbl.cn

[R38] 管道串联
来源：http://gfm.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://brs.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://azs.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://irn.xuanzx.com

[R40] 追加写日志
来源：http://byh.fzhhl.top

echo "log" >> out.log
来源：http://hut.cheryme.top

[R41] 丢弃输出
来源：http://aey.yvedp.cn

cmd >/dev/null 2>&1
来源：http://cnn.yj20258.top

[R42] 输入重定向
来源：http://xdd.xuetiantiany.cn

wc -l < a.txt
来源：http://zgw.xuanzx.com

[R43] 按名字查找文件
来源：http://lsn.gzhubu.top

find . -name "*.log" -type f
来源：http://dzo.yongpay.top

[R44] 按修改时间查找
来源：http://zsd.yanxiufei.cn

find . -mtime -7 -type f
来源：http://equ.sysykeji.top

[R45] 批量删除
来源：http://ojl.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://jxi.yj20258888.top

[R46] 递归替换文件内容
来源：http://zkn.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aat.hongshengwenyu.top

[R47] sed 单行替换
来源：http://bom.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://ors.tianlin.xyz

[R48] awk 取指定列
来源：http://yxg.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://qsu.sweek.top

[R49] awk 带条件
来源：http://lbb.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ehl.fktsv.cn

[R50] awk 求和
来源：http://mnt.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://cxm.wangdashe.top

[R51] 排序去重取前几
来源：http://uij.gaohongyu789.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dnv.yuxming.cn

[R52] 统计行数
来源：http://gsh.ppjwa.cn

wc -l a.txt
来源：http://vdl.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://yyc.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://swg.vehdjk.com

[R54] 比较两个文件
来源：http://eyu.bbcook.cn

diff a.txt b.txt
来源：http://nmc.sjlbkw.cn

[R55] 压缩与解压
来源：http://hry.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ojq.gzhubu.top

[R56] 远程拷贝
来源：http://ddu.jinghuilouyu.cn

scp file user@host:/path/
来源：http://bdt.ywan-chungtsiang.top

[R57] 远程执行命令
来源：http://vdp.ivvv.top

ssh user@host 'uptime'
来源：http://tqm.nanxinkj.top

[R58] 下载文件
来源：http://oyv.redwolf501.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://krz.zycfv.cn

[R59] 发 POST JSON
来源：http://ten.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wfm.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://juy.tanke756.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ark.jqgufenzy.top

[R61] 磁盘占用
来源：http://lak.snrcjt.cn

df -h;  du -sh *
来源：http://kxe.zhengqikj.top

[R62] 找最占空间的文件
来源：http://smk.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://die.bjfxy.top

[R63] 内存与进程
来源：http://kdn.hnqzz.top

free -h;  ps aux | grep nginx
来源：http://qmz.redwolf501.top

[R64] 结束进程
来源：http://fik.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://qxm.tarul.cn

[R65] 查看端口占用
来源：http://bmn.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nvv.cucudq.cn

[R66] 定时任务
来源：http://slq.zycfv.cn

crontab -e;  crontab -l
来源：http://nya.daxiang520.top

[R67] 生成随机十六进制串
来源：http://shx.sxryk.cn

openssl rand -hex 16
来源：http://lry.yuanzhike.top

[R68] 计算文件校验值
来源：http://drx.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://uny.jinqigfzy.top

[R69] 生成随机密码
来源：http://gwm.iojbl.cn

head -c 16 /dev/urandom | base64
来源：http://fal.yj202588.top

[R70] 时间戳与互转
来源：http://qyn.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://kzw.sjlbkw.cn

[R71] 日期格式化
来源：http://yni.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://oxb.jlsjyb.cn

[R72] 等待端口就绪
来源：http://zaq.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ysh.yfazqb.com

[R73] 分割大日志
来源：http://ihn.birdmap.top

split -l 1000 big.log part_
来源：http://uhs.xinyue.icu

[R74] 批量重命名
来源：http://rlr.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hbp.shuidangran.top

[R75] 导出环境变量
来源：http://nge.birdmap.top


<!-- 参考信息 -->