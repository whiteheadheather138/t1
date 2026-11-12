代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://kbd.cucudq.cn

[Q22] 排序
来源：http://bvt.gogol.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fvq.yuxming.cn

[Q23] 分页
来源：http://zxe.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fbn.shuidangran.top

[Q24] 去重
来源：http://bej.ydzc1.top

SELECT DISTINCT city FROM users;
来源：http://zls.iojbl.cn

[Q25] 只取前 N 条
来源：http://wjv.hesvh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qnt.feifeiyinyue.top

[Q26] 计数
来源：http://bib.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://xfl.sjlbkw.cn

[Q27] 条件计数
来源：http://dii.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ysi.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://rpn.chenzaomai.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://krk.guowangkeji.top

[Q29] 最大最小值
来源：http://axk.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bza.yj202588.top

[Q30] 分组统计
来源：http://inv.dianchejie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rfd.ybcxt.top

[Q31] 分组后过滤
来源：http://dbq.mhx1999.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hhm.meibo888.top

[Q32] 分组拼接字符串
来源：http://dim.daxiang520.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gwg.yonumen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bnq.cqqwz.cn

[Q33] 多列分组
来源：http://sqw.ydzc1.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oxv.haohaochexian.top

[Q34] 每组取第一条
来源：http://zli.ywan-chungtsiang.top

SELECT * FROM (
来源：http://eyw.daxiang520.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qpm.haohaochexian.top

) t WHERE rn = 1;
来源：http://ysz.hfpthk.cn

[Q35] 内连接
来源：http://mpp.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xnp.sxryk.cn

[Q36] 左连接
来源：http://rsk.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://akz.shangyingyoupin.top

[Q37] 右连接
来源：http://cek.ydjk.org.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ehl.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://zoq.jqgfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qvx.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://qma.bjfxy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jgw.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kfp.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uzz.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zfh.tarul.cn

[Q41] 多表连接
来源：http://kta.jinqigufen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://auz.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://jki.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://vxr.bbcook.cn

[Q42] 连接条件附加过滤
来源：http://lug.chenzaomai.com

SELECT u.name, o.amount FROM users u
来源：http://etb.meibo888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pqd.xuetiantiany.cn

[Q43] 标量子查询
来源：http://qsf.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bje.xinyue.icu

[Q44] IN 子查询
来源：http://jsi.wangdashe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uyu.ywan-chungtsiang.top

[Q45] EXISTS 判断存在
来源：http://puv.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fqp.hfpthk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sdr.smart0.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://coc.fehbvm.com

[Q47] 与平均值比较
来源：http://sbs.cqqwz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pzg.zhixingplan.top

[Q48] CTE 公用表表达式
来源：http://gdr.ppjwa.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rzg.snrcjt.cn

SELECT * FROM t WHERE c > 5;
来源：http://ubc.fehbvm.com

[Q49] 更新单行
来源：http://ynl.hfpthk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kqk.52xcode.cn

[Q50] 批量更新
来源：http://htg.hnxiangtu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wrl.fengsongda.top

[Q51] 用子查询更新
来源：http://ehc.sysykeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yjn.iojbl.cn

[Q52] 删除指定行
来源：http://gbx.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://jvz.fktsv.cn

[Q53] 按条件删除
来源：http://xxg.jqgufenzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gpx.mhx1999.top

[Q54] 清空表
来源：http://bvh.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://vne.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://lnx.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fjd.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://idp.vqdsnc.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bjn.nanxuanxn.top

[Q57] 行号
来源：http://cll.zhiwuduotai.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uzl.yvedp.cn

[Q58] 累计求和
来源：http://del.jiagoushi.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vzz.vehdjk.com

[Q59] 分组内累计
来源：http://awb.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fws.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://bxp.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zvr.aibaodan.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://czd.c1oappe.top

[Q61] 移动平均
来源：http://kpf.sxryk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zkz.pengpengdd.cyou

[Q62] 分组占比
来源：http://xml.0kj1m.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xgs.smart0.xyz

[Q63] 开启事务
来源：http://fuk.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ubb.yj202588.top

[Q64] 提交事务
来源：http://hmx.hammf.cn

COMMIT;
来源：http://skq.jianghu66.top

[Q65] 回滚事务
来源：http://bdt.ehwqpu.com

ROLLBACK;
来源：http://owa.svipenyu.cn

[Q66] 行锁查询
来源：http://yfs.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mhe.tianlin.xyz

[Q67] 设置隔离级别
来源：http://ooh.haohaochexian.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cux.shanyushiyangtech.top

[Q68] 保存点
来源：http://mmv.yvedp.cn

SAVEPOINT sp1;
来源：http://dia.hfpthk.cn

ROLLBACK TO sp1;
来源：http://avt.ydzc1.top

[Q69] 查看执行计划
来源：http://sxr.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://urn.cucudq.cn

[Q70] 更新统计信息
来源：http://xkb.yueranfly.top

ANALYZE TABLE users;
来源：http://ntw.bbcook.cn

[Q71] 查看建表语句
来源：http://kbx.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lgp.haohaochexian.top

[Q72] 查看索引
来源：http://fgi.yfazqb.com

SHOW INDEX FROM users;
来源：http://yob.52xcode.cn

[Q73] 查看表状态
来源：http://ntr.jlsjyb.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cuw.chenzaomai.com

[Q74] 强制使用索引
来源：http://pem.jinqigufen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ewi.kuanghao11.cn

[Q75] 日期格式化
来源：http://orb.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hdm.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dem.sweek.top

[Q76] 按天统计
来源：http://zra.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pco.chenzaomai.com

[Q77] 时间加减
来源：http://poa.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qgg.fengsongda.top

[Q78] 当前时间
来源：http://fyf.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://epf.fehbvm.com

[Q79] 字符串拼接
来源：http://blh.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mdi.ctjpmb.com

[Q80] 字符串截取
来源：http://xel.sufxvd.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kdt.iojbl.cn

[Q81] 字符串替换
来源：http://ovi.fktsv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nua.jinqigufen.top

[Q82] 字符长度与字节长度
来源：http://syu.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kne.fengsongda.top

[Q83] 大小写转换
来源：http://ypw.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cuc.cheryme.top

[Q84] 去除首尾空格
来源：http://wmu.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://wuq.ivvv.top

[Q85] 数值取整
来源：http://pot.meibo888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pvo.zhengqikj.top

[Q86] 读取 JSON 字段
来源：http://rqg.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bwv.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://zbw.yangfankeji.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://goj.ydjk.org.cn

[Q88] 行转列（条件聚合）
来源：http://zuy.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pkv.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uyx.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://uns.yfazqb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://twm.chenzaomai.com

[Q90] 生成序号列
来源：http://bir.shanyushiyangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gzh.nanxinkj.top

================================================================================
来源：http://lbb.fzhhl.top

R. Bash 专题
来源：http://fkj.wangdashe.top

================================================================================
来源：http://nel.ydjk.org.cn

[R01] shebang 与严格模式
来源：http://uoy.chenlongwang.top

#!/usr/bin/env bash
来源：http://zjv.cdnleiting.top

set -euo pipefail
来源：http://ppv.hcnkem.com

[R02] 变量赋值与使用
来源：http://zbg.tanke756.top

name="Tom"; echo "$name"
来源：http://ybu.yj20258.top

[R03] 只读变量
来源：http://yfm.zdbjq.cn

readonly PI=3.14
来源：http://fnr.zdbjq.cn

[R04] 位置参数
来源：http://iww.zhaomingkeji.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hey.sufxvd.cn

[R05] 参数默认值
来源：http://emi.chenlongwang.top

name="${1:-default}"
来源：http://eia.xuanzx.com

[R06] 判断命令是否存在
来源：http://qke.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gty.guowangkeji.top

[R07] if 判断文件
来源：http://snf.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tta.jinqigufen.top

[R08] 数值比较
来源：http://tna.zhengqikj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jqy.hfpthk.cn

[R09] 字符串比较
来源：http://vpq.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kkh.daria6918.cn

[R10] 正则匹配
来源：http://nfo.xylfe.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cns.jqgfzy.top

[R11] case 多分支
来源：http://lzl.wangshuangyany.cn

case "$1" in
来源：http://lgx.jlsjyb.cn

start) echo "启动" ;;
来源：http://hco.ywan-chungtsiang.top

stop)  echo "停止" ;;
来源：http://ajf.nwbrower.top

*)     echo "未知命令" ;;
来源：http://cdj.cqqwz.cn

esac
来源：http://jua.pycfn.com

[R12] for 遍历文件
来源：http://kil.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://ksw.fengsongda.top

[R13] for 计数循环
来源：http://uxf.smart0.xyz

for i in {1..10}; do echo "$i"; done
来源：http://qbz.52xcode.cn

[R14] C 风格 for
来源：http://vky.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jil.yuanzhike.top

[R15] while 逐行读文件
来源：http://pid.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tlx.hysaishi.cn

[R16] until 等待条件
来源：http://dhd.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bhc.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://cyc.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://esw.daxiang520.top

[R18] 遍历数组
来源：http://liu.yj20258.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aqv.yanxiufei.cn

[R19] 数组长度
来源：http://wzd.hysaishi.cn

echo "${#arr[@]}"
来源：http://prs.sxryk.cn

[R20] 关联数组（字典）
来源：http://vie.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://prp.vqdsnc.cn

[R21] 字符串长度
来源：http://ams.yangfankeji.com

echo "${#s}"
来源：http://yjf.cdnleiting.top

[R22] 截取子串
来源：http://vmk.wangdashe.top

echo "${s:0:5}"
来源：http://czc.sufxvd.cn

[R23] 字符串替换
来源：http://evj.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ugj.jlsjyb.cn

[R24] 大小写转换
来源：http://ive.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://djd.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://mia.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://pjc.zhijiandao.cn

[R26] 命令替换
来源：http://lbt.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://yuf.gogol.net.cn

[R27] 算术展开
来源：http://jmc.pycfn.com

echo $((1 + 2 * 3))
来源：http://bjo.smart0.xyz

[R28] 浮点运算
来源：http://dsx.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://ssj.nanxinkj.top

[R29] 定义函数
来源：http://yzz.jinqigfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ymq.zhijiandao.cn

[R30] 函数返回状态码
来源：http://qzj.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://brs.yangfankeji.com

[R31] 局部变量
来源：http://zrd.xuanzx.com

f() { local x=1; echo "$x"; }
来源：http://dus.hfpthk.cn

[R32] 参数个数校验
来源：http://gki.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://htb.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://uti.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dtx.svipenyu.cn

[R34] 退出时清理
来源：http://tsy.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://vvc.yongpay.top

[R35] 后台执行并等待
来源：http://dzx.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xkc.hammf.cn

[R36] 并发执行多个任务
来源：http://baj.gaohongyu789.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xsf.bbcook.cn

[R37] 把输出赋给变量
来源：http://ndv.zhixingplan.top

files=$(ls -1)
来源：http://tyb.hysaishi.cn

[R38] 管道串联
来源：http://sfj.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://med.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://xpi.yj202588.top

cmd > out.log 2>&1
来源：http://dwi.yj20258.top

[R40] 追加写日志
来源：http://jfr.fanxiaobao.xyz

echo "log" >> out.log
来源：http://vhu.gaohongyu789.top

[R41] 丢弃输出
来源：http://vcp.hnqzz.top

cmd >/dev/null 2>&1
来源：http://ksv.jinqigufen.top

[R42] 输入重定向
来源：http://mvg.yongpay.top

wc -l < a.txt
来源：http://pdr.tianlin.xyz

[R43] 按名字查找文件
来源：http://qiq.zhiwuduotai.top

find . -name "*.log" -type f
来源：http://ytg.uphjek.com

[R44] 按修改时间查找
来源：http://hdh.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://iru.9152youxi.cn

[R45] 批量删除
来源：http://itr.hesvh.cn

find . -name "*.tmp" -delete
来源：http://dsw.xinyue.icu

[R46] 递归替换文件内容
来源：http://xgw.smart0.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uyj.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://vgw.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://efx.daxiang520.top

[R48] awk 取指定列
来源：http://oms.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://plp.iojbl.cn

[R49] awk 带条件
来源：http://snx.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gqg.andypj.xyz

[R50] awk 求和
来源：http://tnf.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rjq.tianlin.xyz

[R51] 排序去重取前几
来源：http://pau.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rup.nanxuanxn.top

[R52] 统计行数
来源：http://wac.xuetiantiany.cn

wc -l a.txt
来源：http://oac.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://uvj.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qjy.yj20258888.top

[R54] 比较两个文件
来源：http://laf.redwolf501.top

diff a.txt b.txt
来源：http://ima.tarul.cn

[R55] 压缩与解压
来源：http://ool.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yww.shzxlz.cn

[R56] 远程拷贝
来源：http://uim.hfpthk.cn

scp file user@host:/path/
来源：http://fog.pycfn.com

[R57] 远程执行命令
来源：http://oqw.jqgfzy.top

ssh user@host 'uptime'
来源：http://uop.xinyue.icu

[R58] 下载文件
来源：http://xsp.zhiwuduotai.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://owp.hnxiangtu.top

[R59] 发 POST JSON
来源：http://fya.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oqa.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://qzy.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pvi.smart0.xyz

[R61] 磁盘占用
来源：http://kzf.52xcode.cn

df -h;  du -sh *
来源：http://cqr.hammf.cn

[R62] 找最占空间的文件
来源：http://xbe.uphjek.com

du -ah . | sort -rh | head -10
来源：http://mvo.sjlbkw.cn

[R63] 内存与进程
来源：http://mzw.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://whs.andypj.xyz

[R64] 结束进程
来源：http://hnn.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://glz.feifeiyinyue.top

[R65] 查看端口占用
来源：http://bbp.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://veu.sjlbkw.cn

[R66] 定时任务
来源：http://ztx.bjfxy.top

crontab -e;  crontab -l
来源：http://szc.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://lta.feifeiyinyue.top

openssl rand -hex 16
来源：http://xit.dianchejie.cn

[R68] 计算文件校验值
来源：http://baa.fktsv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yqy.wangshuangyany.cn

[R69] 生成随机密码
来源：http://bvs.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://jki.wangdashe.top

[R70] 时间戳与互转
来源：http://zwu.ybcxt.top

date +%s;  date -d @1700000000
来源：http://dcy.hysaishi.cn

[R71] 日期格式化
来源：http://rhh.tanke756.top


<!-- 参考信息 -->