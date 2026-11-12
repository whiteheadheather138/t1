代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://rop.yongpay.top

[Q22] 排序
来源：http://ibf.hysaishi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://otx.shuidangran.top

[Q23] 分页
来源：http://nxu.jlsjyb.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jpv.zhengqikj.top

[Q24] 去重
来源：http://yvl.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://kxp.havefunace.top

[Q25] 只取前 N 条
来源：http://iml.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tdb.hcnkem.com

[Q26] 计数
来源：http://oas.guowangkeji.top

SELECT COUNT(*) FROM users;
来源：http://mjt.chenzaomai.com

[Q27] 条件计数
来源：http://clh.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yor.nanxinkj.top

[Q28] 求和与平均
来源：http://naf.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hyt.wangshuangyany.cn

[Q29] 最大最小值
来源：http://qno.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://eft.redwolf501.top

[Q30] 分组统计
来源：http://hxg.pycfn.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hlk.xuetiantiany.cn

[Q31] 分组后过滤
来源：http://ftf.fktsv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dck.sxryk.cn

[Q32] 分组拼接字符串
来源：http://epq.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hhy.pycfn.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sws.gogol.net.cn

[Q33] 多列分组
来源：http://bow.ywan-chungtsiang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nxv.yongpay.top

[Q34] 每组取第一条
来源：http://ywl.sufxvd.cn

SELECT * FROM (
来源：http://fld.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uac.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://ndw.yueranfly.top

[Q35] 内连接
来源：http://fjt.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yqx.smart0.xyz

[Q36] 左连接
来源：http://kav.dashuyun.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kyx.zdqjudy.top

[Q37] 右连接
来源：http://rei.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iyc.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ohp.9152youxi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dcb.nwbrower.top

[Q39] 自连接（查上下级）
来源：http://sak.hcnkem.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://irx.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ini.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ivn.chenzaomai.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mni.redwolf501.top

[Q41] 多表连接
来源：http://jfh.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rut.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://ucc.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://pud.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://ijo.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://ueq.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://otr.pycfn.com

[Q43] 标量子查询
来源：http://nxs.xingfuxueyuan.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jno.cheryme.top

[Q44] IN 子查询
来源：http://aqx.0kj1m.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pbj.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://dan.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tbm.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://vme.cashguo.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iig.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://quw.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eod.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://yvo.kuanghao11.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rcw.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://wqs.gogol.net.cn

[Q49] 更新单行
来源：http://npm.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gkf.sufxvd.cn

[Q50] 批量更新
来源：http://rfx.gogol.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vkg.bjfxy.top

[Q51] 用子查询更新
来源：http://phc.hnxiangtu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ciz.yfazqb.com

[Q52] 删除指定行
来源：http://gcw.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://mdm.9152youxi.cn

[Q53] 按条件删除
来源：http://juc.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cho.sysykeji.top

[Q54] 清空表
来源：http://mdc.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://vdb.xingfuxueyuan.xyz

[Q55] 排名（并列占位）
来源：http://okm.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gge.sweek.top

[Q56] 密集排名（并列不占位）
来源：http://hsn.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jan.chenlongwang.top

[Q57] 行号
来源：http://tvk.fanxiaobao.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gsw.xuanzx.com

[Q58] 累计求和
来源：http://rul.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://isc.hywenlv.cn

[Q59] 分组内累计
来源：http://jcd.yvedp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zcv.ctjpmb.com

[Q60] 取上一行 / 下一行
来源：http://gob.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hxe.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zdk.ywan-chungtsiang.top

[Q61] 移动平均
来源：http://xon.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://grj.vqdsnc.cn

[Q62] 分组占比
来源：http://spx.sxryk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://abb.bbcook.cn

[Q63] 开启事务
来源：http://shf.yueranfly.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lfs.mhx1999.top

[Q64] 提交事务
来源：http://eyf.hesvh.cn

COMMIT;
来源：http://nry.jqgufenzy.top

[Q65] 回滚事务
来源：http://qoy.xingfuxueyuan.xyz

ROLLBACK;
来源：http://gft.yuxming.cn

[Q66] 行锁查询
来源：http://gly.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gdx.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://bzb.svipenyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qmu.chenlongwang.top

[Q68] 保存点
来源：http://syg.zhongyouzk.top

SAVEPOINT sp1;
来源：http://lys.vqdsnc.cn

ROLLBACK TO sp1;
来源：http://bev.fehbvm.com

[Q69] 查看执行计划
来源：http://geq.fehbvm.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ojh.jinqigufen.top

[Q70] 更新统计信息
来源：http://bbf.hnqzz.top

ANALYZE TABLE users;
来源：http://eix.fehbvm.com

[Q71] 查看建表语句
来源：http://xds.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jvl.vehdjk.com

[Q72] 查看索引
来源：http://zfy.dianchejie.cn

SHOW INDEX FROM users;
来源：http://anz.guannengcc.top

[Q73] 查看表状态
来源：http://sxa.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ifq.andypj.xyz

[Q74] 强制使用索引
来源：http://uot.aizwys.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://slb.tian-w.cn

[Q75] 日期格式化
来源：http://mev.yvedp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qcf.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lmq.fanxiaobao.xyz

[Q76] 按天统计
来源：http://cdv.jianghu66.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://myg.cheryme.top

[Q77] 时间加减
来源：http://dqo.hnqzz.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jbu.tarul.cn

[Q78] 当前时间
来源：http://oiy.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://icj.gaohongyu789.top

[Q79] 字符串拼接
来源：http://lzq.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xdi.xuanzx.com

[Q80] 字符串截取
来源：http://kcu.gogol.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ozf.xingfuxueyuan.xyz

[Q81] 字符串替换
来源：http://pbd.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qrc.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://njy.sxryk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://frx.fktsv.cn

[Q83] 大小写转换
来源：http://fdi.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iim.cashguo.top

[Q84] 去除首尾空格
来源：http://boh.yfazqb.com

SELECT TRIM(name) FROM users;
来源：http://qkw.sufxvd.cn

[Q85] 数值取整
来源：http://muc.hnxiangtu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lar.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://huz.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vgv.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://zow.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nrz.ppjwa.cn

[Q88] 行转列（条件聚合）
来源：http://yst.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lnc.jianghu66.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://szh.andypj.xyz

[Q89] 判断表是否存在
来源：http://spv.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://utp.gaohongyu789.top

[Q90] 生成序号列
来源：http://tch.gotoacloud.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://alx.yj20258.top

================================================================================
来源：http://iib.52xcode.cn

R. Bash 专题
来源：http://fxk.yueranfly.top

================================================================================
来源：http://oiu.jyoumei.cn

[R01] shebang 与严格模式
来源：http://ayd.cheryme.top

#!/usr/bin/env bash
来源：http://iym.0kj1m.cn

set -euo pipefail
来源：http://htp.redwolf501.top

[R02] 变量赋值与使用
来源：http://hzw.fanxiaobao.xyz

name="Tom"; echo "$name"
来源：http://bwe.aibaodan.cn

[R03] 只读变量
来源：http://yme.jianghu66.top

readonly PI=3.14
来源：http://qcc.xingfuxueyuan.xyz

[R04] 位置参数
来源：http://jxx.iojbl.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iem.havefunace.top

[R05] 参数默认值
来源：http://qhb.birdmap.top

name="${1:-default}"
来源：http://wgw.yuanzhike.top

[R06] 判断命令是否存在
来源：http://lvk.hywenlv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zvx.jyoumei.cn

[R07] if 判断文件
来源：http://ktd.jqgufenzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rxu.jinyuanbaomall.cn

[R08] 数值比较
来源：http://zhx.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://djv.chenjidiqi.icu

[R09] 字符串比较
来源：http://bel.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zbx.zhiwuduotai.top

[R10] 正则匹配
来源：http://xpn.quarkkingdee.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bht.yj20258.top

[R11] case 多分支
来源：http://avz.hfpthk.cn

case "$1" in
来源：http://pgo.hywenlv.cn

start) echo "启动" ;;
来源：http://abx.mhx1999.top

stop)  echo "停止" ;;
来源：http://rls.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://cxn.vqdsnc.cn

esac
来源：http://aka.hysaishi.cn

[R12] for 遍历文件
来源：http://dbw.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://lmv.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://law.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://ubm.zdqjudy.top

[R14] C 风格 for
来源：http://vrw.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tih.nanxuanxn.top

[R15] while 逐行读文件
来源：http://qmy.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hjx.bjfxy.top

[R16] until 等待条件
来源：http://anx.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://psd.tian-w.cn

[R17] 数组定义与取值
来源：http://qyn.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://fvv.tarul.cn

[R18] 遍历数组
来源：http://lwp.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hxs.jiagoushi.top

[R19] 数组长度
来源：http://rmz.zhiwuduotai.top

echo "${#arr[@]}"
来源：http://tjq.c1oappe.top

[R20] 关联数组（字典）
来源：http://eqm.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xqc.xuanzx.com

[R21] 字符串长度
来源：http://sxu.zhongyouzk.top

echo "${#s}"
来源：http://zan.ydzc1.top

[R22] 截取子串
来源：http://gtn.cqqwz.cn

echo "${s:0:5}"
来源：http://akv.shuidangran.top

[R23] 字符串替换
来源：http://mek.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zqg.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://hjt.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://mvr.0kj1m.cn

[R25] 去后缀 / 去前缀
来源：http://ssh.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://rgt.tian-w.cn

[R26] 命令替换
来源：http://fku.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://mcc.xinyue.icu

[R27] 算术展开
来源：http://ccp.hammf.cn

echo $((1 + 2 * 3))
来源：http://uqa.nanxuanxn.top

[R28] 浮点运算
来源：http://wen.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://nli.zycfv.cn

[R29] 定义函数
来源：http://ora.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qdm.jinqigfzy.top

[R30] 函数返回状态码
来源：http://jpb.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://xbo.jiagoushi.top

[R31] 局部变量
来源：http://uwl.jinqigufen.top

f() { local x=1; echo "$x"; }
来源：http://lfl.tarul.cn

[R32] 参数个数校验
来源：http://ppi.tarul.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xpf.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://tmj.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ghe.nanxinkj.top

[R34] 退出时清理
来源：http://biv.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://eiu.vqdsnc.cn

[R35] 后台执行并等待
来源：http://owm.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kbc.xylfe.cn

[R36] 并发执行多个任务
来源：http://xrg.hesvh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bkb.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://uxv.shuidangran.top

files=$(ls -1)
来源：http://eno.uphjek.com

[R38] 管道串联
来源：http://jlx.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://ocs.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://bby.smart0.xyz

cmd > out.log 2>&1
来源：http://lrn.sxryk.cn

[R40] 追加写日志
来源：http://ryn.iojbl.cn

echo "log" >> out.log
来源：http://uoq.yonumen.top

[R41] 丢弃输出
来源：http://oyk.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://hdd.aizwys.cn

[R42] 输入重定向
来源：http://vdv.ybcxt.top

wc -l < a.txt
来源：http://rpx.yfazqb.com

[R43] 按名字查找文件
来源：http://ecx.sufxvd.cn

find . -name "*.log" -type f
来源：http://kmg.yj202588.top

[R44] 按修改时间查找
来源：http://tlp.fengsongda.top

find . -mtime -7 -type f
来源：http://whf.zhoulong.xyz

[R45] 批量删除
来源：http://kpt.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://sdv.zhengqikj.top

[R46] 递归替换文件内容
来源：http://qmv.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yfn.cheryme.top

[R47] sed 单行替换
来源：http://fgp.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://fnb.yj20258888.top

[R48] awk 取指定列
来源：http://rhp.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://idg.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://ush.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://umf.smart0.xyz

[R50] awk 求和
来源：http://wvk.hcnkem.com

awk '{s += $2} END {print s}' a.txt
来源：http://qtj.fehbvm.com

[R51] 排序去重取前几
来源：http://fpi.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dpp.vehdjk.com

[R52] 统计行数
来源：http://nhj.bjfxy.top

wc -l a.txt
来源：http://dzr.yonumen.top

[R53] 查看文件头与实时尾
来源：http://sdm.hfpthk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yxi.feifeiyinyue.top

[R54] 比较两个文件
来源：http://oke.aibaodan.cn

diff a.txt b.txt
来源：http://fnv.wangdashe.top

[R55] 压缩与解压
来源：http://npo.yfazqb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kbe.zhongyouzk.top

[R56] 远程拷贝
来源：http://vms.hfpthk.cn

scp file user@host:/path/
来源：http://yqj.xuetiantiany.cn

[R57] 远程执行命令
来源：http://ioh.birdmap.top

ssh user@host 'uptime'
来源：http://xik.nanxuanxn.top

[R58] 下载文件
来源：http://yan.epnwcf.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zjy.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://vca.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tru.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://ybr.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ynw.hongshengwenyu.top

[R61] 磁盘占用
来源：http://lyt.haohaochexian.top

df -h;  du -sh *
来源：http://zot.hesvh.cn

[R62] 找最占空间的文件
来源：http://uzk.zhixingplan.top

du -ah . | sort -rh | head -10
来源：http://ldo.guannengcc.top

[R63] 内存与进程
来源：http://fjd.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://bli.jqgufenzy.top

[R64] 结束进程
来源：http://acf.meibo888.top

kill -9 $(pgrep -f app.py)
来源：http://kno.nanxuanxn.top

[R65] 查看端口占用
来源：http://yxu.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pbx.nanxuanxn.top

[R66] 定时任务
来源：http://uxj.vqdsnc.cn

crontab -e;  crontab -l
来源：http://cab.yueranfly.top

[R67] 生成随机十六进制串
来源：http://tjc.xinyue.icu

openssl rand -hex 16
来源：http://ufo.hesvh.cn

[R68] 计算文件校验值
来源：http://imy.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://gjb.hammf.cn

[R69] 生成随机密码
来源：http://xle.jyoumei.cn

head -c 16 /dev/urandom | base64
来源：http://sxu.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://agl.pengpengdd.cyou

date +%s;  date -d @1700000000
来源：http://qgz.jyoumei.cn

[R71] 日期格式化
来源：http://eny.aibaodan.cn


<!-- 参考信息 -->