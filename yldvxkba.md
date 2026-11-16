代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kws.havefunace.top

[Q24] 去重
来源：http://bgt.ppjwa.cn

SELECT DISTINCT city FROM users;
来源：http://jeo.yj20258.top

[Q25] 只取前 N 条
来源：http://tpt.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aee.wangshuangyany.cn

[Q26] 计数
来源：http://mql.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://blx.gzhubu.top

[Q27] 条件计数
来源：http://kxp.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ygz.svipenyu.cn

[Q28] 求和与平均
来源：http://lrx.nanxinkj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fym.guowangkeji.top

[Q29] 最大最小值
来源：http://kuw.zhijiandao.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jed.jqgufenzy.top

[Q30] 分组统计
来源：http://eki.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nyi.svipenyu.cn

[Q31] 分组后过滤
来源：http://zoa.snrcjt.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yzw.shzxlz.cn

[Q32] 分组拼接字符串
来源：http://rfn.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ntz.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://owr.nwbrower.top

[Q33] 多列分组
来源：http://gax.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qvf.quarkkingdee.top

[Q34] 每组取第一条
来源：http://swv.ydjk.org.cn

SELECT * FROM (
来源：http://dwj.havefunace.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lsr.jianghu66.top

) t WHERE rn = 1;
来源：http://iip.tanke756.top

[Q35] 内连接
来源：http://kfe.yueranfly.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lxp.zdbjq.cn

[Q36] 左连接
来源：http://gej.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jtp.cdnleiting.top

[Q37] 右连接
来源：http://opp.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gyt.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cpu.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gue.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://cea.cucudq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://etj.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xae.xuanzx.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ieb.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fum.chenzaomai.com

[Q41] 多表连接
来源：http://nmq.hesvh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dhx.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://prs.jinyuanbaomall.cn

JOIN products p ON p.id = o.product_id;
来源：http://qef.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://rtg.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://mhm.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bmf.zdqjudy.top

[Q43] 标量子查询
来源：http://gkq.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dnw.guannengcc.top

[Q44] IN 子查询
来源：http://ngo.sweek.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mio.ywan-chungtsiang.top

[Q45] EXISTS 判断存在
来源：http://ecc.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nks.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zyu.sxryk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tht.jinqigufen.top

[Q47] 与平均值比较
来源：http://ybp.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pkj.havefunace.top

[Q48] CTE 公用表表达式
来源：http://wce.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xer.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://dbs.snrcjt.cn

[Q49] 更新单行
来源：http://hwx.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hlu.c1oappe.top

[Q50] 批量更新
来源：http://gri.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cfy.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://tcj.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pua.ybcxt.top

[Q52] 删除指定行
来源：http://ulq.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://uhc.iojbl.cn

[Q53] 按条件删除
来源：http://hhc.snrcjt.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qhg.feifeiyinyue.top

[Q54] 清空表
来源：http://zyf.pycfn.com

TRUNCATE TABLE logs;
来源：http://wnl.zdbjq.cn

[Q55] 排名（并列占位）
来源：http://pva.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://evg.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://sxn.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nct.cucudq.cn

[Q57] 行号
来源：http://pvk.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cix.meibo888.top

[Q58] 累计求和
来源：http://bta.zhongyouzk.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wkk.yj20258888.top

[Q59] 分组内累计
来源：http://whd.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gft.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://uxq.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tqy.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://szk.shuidangran.top

[Q61] 移动平均
来源：http://gkr.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lty.uphjek.com

[Q62] 分组占比
来源：http://xjx.fzhhl.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wjr.tarul.cn

[Q63] 开启事务
来源：http://hkh.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://owl.jyoumei.cn

[Q64] 提交事务
来源：http://mbs.hnxiangtu.top

COMMIT;
来源：http://nnc.cdnleiting.top

[Q65] 回滚事务
来源：http://yps.bjfxy.top

ROLLBACK;
来源：http://bsy.yangfankeji.com

[Q66] 行锁查询
来源：http://fbp.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ldk.ydzc1.top

[Q67] 设置隔离级别
来源：http://auy.ivvv.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pgs.hcnkem.com

[Q68] 保存点
来源：http://xzn.dashuyun.cn

SAVEPOINT sp1;
来源：http://sdn.wangshuangyany.cn

ROLLBACK TO sp1;
来源：http://lzf.yongpay.top

[Q69] 查看执行计划
来源：http://cmp.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dmg.shanyushiyangtech.top

[Q70] 更新统计信息
来源：http://sok.jqgufenzy.top

ANALYZE TABLE users;
来源：http://cih.tian-w.cn

[Q71] 查看建表语句
来源：http://hxb.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vrm.sysykeji.top

[Q72] 查看索引
来源：http://vle.tianlin.xyz

SHOW INDEX FROM users;
来源：http://crh.ctjpmb.com

[Q73] 查看表状态
来源：http://hxw.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://owx.cashguo.top

[Q74] 强制使用索引
来源：http://fzw.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://end.gotoacloud.top

[Q75] 日期格式化
来源：http://khj.shuidangran.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ymc.sysykeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xyo.pycfn.com

[Q76] 按天统计
来源：http://mqm.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cbb.shangyingyoupin.top

[Q77] 时间加减
来源：http://hnw.cdnleiting.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sos.zhijiandao.cn

[Q78] 当前时间
来源：http://cye.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://han.jlsjyb.cn

[Q79] 字符串拼接
来源：http://lwa.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uwz.shangyingyoupin.top

[Q80] 字符串截取
来源：http://pbz.tanke756.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fea.yuanzhike.top

[Q81] 字符串替换
来源：http://ifu.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fkr.jinqigufen.top

[Q82] 字符长度与字节长度
来源：http://qzf.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xay.yonumen.top

[Q83] 大小写转换
来源：http://mdk.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rlx.jqgfzy.top

[Q84] 去除首尾空格
来源：http://ztu.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://qkg.yfazqb.com

[Q85] 数值取整
来源：http://vrs.hammf.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vhg.jiagoushi.top

[Q86] 读取 JSON 字段
来源：http://xgc.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fda.fanxiaobao.xyz

[Q87] JSON 字段做条件
来源：http://ndk.nanxinkj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xum.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://szn.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bvx.guannengcc.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zll.dashuyun.cn

[Q89] 判断表是否存在
来源：http://mhf.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hud.tianlin.xyz

[Q90] 生成序号列
来源：http://jnm.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ney.daxiang520.top

================================================================================
来源：http://rqd.hysaishi.cn

R. Bash 专题
来源：http://brk.zdbjq.cn

================================================================================
来源：http://bed.nwbrower.top

[R01] shebang 与严格模式
来源：http://mpm.yvedp.cn

#!/usr/bin/env bash
来源：http://vfa.sweek.top

set -euo pipefail
来源：http://lek.daxiang520.top

[R02] 变量赋值与使用
来源：http://nfc.jlsjyb.cn

name="Tom"; echo "$name"
来源：http://wgx.birdmap.top

[R03] 只读变量
来源：http://slp.zhongyouzk.top

readonly PI=3.14
来源：http://ula.zhaomingkeji.xyz

[R04] 位置参数
来源：http://isc.zhaomingkeji.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hke.tian-w.cn

[R05] 参数默认值
来源：http://ydu.fktsv.cn

name="${1:-default}"
来源：http://btb.quarkkingdee.top

[R06] 判断命令是否存在
来源：http://apo.shangyingyoupin.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kpi.nwbrower.top

[R07] if 判断文件
来源：http://oxa.fzhhl.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cfr.nanxuanxn.top

[R08] 数值比较
来源：http://syk.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jri.tian-w.cn

[R09] 字符串比较
来源：http://kxh.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://leb.gzhubu.top

[R10] 正则匹配
来源：http://kco.haohaochexian.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tqa.daria6918.cn

[R11] case 多分支
来源：http://qdi.guannengcc.top

case "$1" in
来源：http://zvb.jqgufenzy.top

start) echo "启动" ;;
来源：http://gry.yangfankeji.com

stop)  echo "停止" ;;
来源：http://mja.aizwys.cn

*)     echo "未知命令" ;;
来源：http://vdn.ppjwa.cn

esac
来源：http://abz.hnxiangtu.top

[R12] for 遍历文件
来源：http://sht.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://noi.smart0.xyz

[R13] for 计数循环
来源：http://lxm.tian-w.cn

for i in {1..10}; do echo "$i"; done
来源：http://udq.pycfn.com

[R14] C 风格 for
来源：http://vto.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zku.gzhubu.top

[R15] while 逐行读文件
来源：http://jra.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kag.aizwys.cn

[R16] until 等待条件
来源：http://xly.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://waf.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://efb.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wmq.xziqi.cn

[R18] 遍历数组
来源：http://kfs.daxiang520.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dnk.cashguo.top

[R19] 数组长度
来源：http://yed.cqqwz.cn

echo "${#arr[@]}"
来源：http://sbx.vehdjk.com

[R20] 关联数组（字典）
来源：http://nya.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fxu.cqqwz.cn

[R21] 字符串长度
来源：http://yzt.wangdashe.top

echo "${#s}"
来源：http://uri.fzhhl.top

[R22] 截取子串
来源：http://rpq.yonumen.top

echo "${s:0:5}"
来源：http://fuq.ehwqpu.com

[R23] 字符串替换
来源：http://pwy.nanxuanxn.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yfk.svipenyu.cn

[R24] 大小写转换
来源：http://vjb.ywan-chungtsiang.top

echo "${s^^}"; echo "${s,,}"
来源：http://jkh.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://ugr.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uvl.tian-w.cn

[R26] 命令替换
来源：http://lzy.andypj.xyz

now=$(date +%F); echo "$now"
来源：http://uox.ctjpmb.com

[R27] 算术展开
来源：http://bbr.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://nxl.9152youxi.cn

[R28] 浮点运算
来源：http://efd.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://hrn.ivvv.top

[R29] 定义函数
来源：http://kxj.mhx1999.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ksb.tanke756.top

[R30] 函数返回状态码
来源：http://iiu.hammf.cn

f() { return 0; }; f || echo "失败了"
来源：http://abp.ctjpmb.com

[R31] 局部变量
来源：http://egx.yangfankeji.com

f() { local x=1; echo "$x"; }
来源：http://yyp.pycfn.com

[R32] 参数个数校验
来源：http://zwy.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dto.vqdsnc.cn

[R33] 捕获错误并提示行号
来源：http://afu.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bga.ehwqpu.com

[R34] 退出时清理
来源：http://xjk.smart0.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://vwv.birdmap.top

[R35] 后台执行并等待
来源：http://qmb.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://del.haohaochexian.top

[R36] 并发执行多个任务
来源：http://wtg.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kpj.52xcode.cn

[R37] 把输出赋给变量
来源：http://ndj.birdmap.top

files=$(ls -1)
来源：http://hek.hysaishi.cn

[R38] 管道串联
来源：http://qjz.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://zpb.hammf.cn

[R39] 重定向标准输出与错误
来源：http://ufo.guannengcc.top

cmd > out.log 2>&1
来源：http://bfx.fehbvm.com

[R40] 追加写日志
来源：http://xxb.jlsjyb.cn

echo "log" >> out.log
来源：http://fjp.xingfuxueyuan.xyz

[R41] 丢弃输出
来源：http://alb.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://qjd.svipenyu.cn

[R42] 输入重定向
来源：http://uud.bbcook.cn

wc -l < a.txt
来源：http://zcn.dashuyun.cn

[R43] 按名字查找文件
来源：http://nhb.wangdashe.top

find . -name "*.log" -type f
来源：http://msw.hysaishi.cn

[R44] 按修改时间查找
来源：http://juc.bjfxy.top

find . -mtime -7 -type f
来源：http://qrs.ydzc1.top

[R45] 批量删除
来源：http://cij.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://rta.ybcxt.top

[R46] 递归替换文件内容
来源：http://hyl.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ipl.wangdashe.top

[R47] sed 单行替换
来源：http://xrm.quarkkingdee.top

sed -i 's/foo/bar/g' a.txt
来源：http://ucg.jyoumei.cn

[R48] awk 取指定列
来源：http://ucl.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://xco.gotoacloud.top

[R49] awk 带条件
来源：http://ray.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fhs.hysaishi.cn

[R50] awk 求和
来源：http://jfr.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cnd.yuanzhike.top

[R51] 排序去重取前几
来源：http://drn.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ajl.jqgufenzy.top

[R52] 统计行数
来源：http://pcn.zhiwuduotai.top

wc -l a.txt
来源：http://zcl.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://zns.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fgy.hywenlv.cn

[R54] 比较两个文件
来源：http://znh.hywenlv.cn

diff a.txt b.txt
来源：http://afz.pengpengdd.cyou

[R55] 压缩与解压
来源：http://pkd.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wys.svipenyu.cn

[R56] 远程拷贝
来源：http://stu.zhiwuduotai.top

scp file user@host:/path/
来源：http://aru.dianchejie.cn

[R57] 远程执行命令
来源：http://zvv.jqgufenzy.top

ssh user@host 'uptime'
来源：http://hse.ehwqpu.com

[R58] 下载文件
来源：http://ijd.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hdu.zhijiandao.cn

[R59] 发 POST JSON
来源：http://oyp.0kj1m.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://irm.aibaodan.cn

[R60] 只看 HTTP 状态码
来源：http://cwy.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://auq.ehwqpu.com

[R61] 磁盘占用
来源：http://drr.pengpengdd.cyou

df -h;  du -sh *
来源：http://zvx.shuidangran.top

[R62] 找最占空间的文件
来源：http://yym.shangyingyoupin.top

du -ah . | sort -rh | head -10
来源：http://pjk.guowangkeji.top

[R63] 内存与进程
来源：http://ouf.pycfn.com

free -h;  ps aux | grep nginx
来源：http://zmt.redwolf501.top

[R64] 结束进程
来源：http://van.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://crt.xylfe.cn

[R65] 查看端口占用
来源：http://gun.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kvg.hesvh.cn

[R66] 定时任务
来源：http://cyb.ybcxt.top

crontab -e;  crontab -l
来源：http://bjv.daxiang520.top

[R67] 生成随机十六进制串
来源：http://xvt.0kj1m.cn

openssl rand -hex 16
来源：http://aye.gaohongyu789.top

[R68] 计算文件校验值
来源：http://yff.sysykeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://gxx.aizwys.cn

[R69] 生成随机密码
来源：http://mbb.tianlin.xyz

head -c 16 /dev/urandom | base64
来源：http://vzg.yj20258888.top

[R70] 时间戳与互转
来源：http://mxz.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://tsq.yonumen.top

[R71] 日期格式化
来源：http://tll.zhaomingkeji.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://hdx.hammf.cn

[R72] 等待端口就绪
来源：http://ffh.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ija.vqdsnc.cn

[R73] 分割大日志
来源：http://xkx.yj202588.top


<!-- 参考信息 -->