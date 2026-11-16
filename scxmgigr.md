代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dex.zycfv.cn

[Q24] 去重
来源：http://myu.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://iub.pycfn.com

[Q25] 只取前 N 条
来源：http://scv.daxiang520.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bfi.hfpthk.cn

[Q26] 计数
来源：http://yho.52xcode.cn

SELECT COUNT(*) FROM users;
来源：http://epi.nanxinkj.top

[Q27] 条件计数
来源：http://bct.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ksr.ybcxt.top

[Q28] 求和与平均
来源：http://ypj.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nyx.shzxlz.cn

[Q29] 最大最小值
来源：http://kbz.zhijiandao.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vus.yonumen.top

[Q30] 分组统计
来源：http://zea.wangdashe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://szh.chenzaomai.com

[Q31] 分组后过滤
来源：http://rqa.daria6918.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yqb.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://cui.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xfv.xuetiantiany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oju.daria6918.cn

[Q33] 多列分组
来源：http://zrk.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mqr.52xcode.cn

[Q34] 每组取第一条
来源：http://apf.chenjidiqi.icu

SELECT * FROM (
来源：http://ila.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gsp.hcnkem.com

) t WHERE rn = 1;
来源：http://yxj.hfpthk.cn

[Q35] 内连接
来源：http://xhw.fehbvm.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://law.nanxuanxn.top

[Q36] 左连接
来源：http://iur.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://czx.hesvh.cn

[Q37] 右连接
来源：http://tik.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bxw.jinghuilouyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dvf.jqgufenzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mjt.hesvh.cn

[Q39] 自连接（查上下级）
来源：http://vdr.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://vgp.ydzc1.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cmk.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://weg.ydjk.org.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://olu.fehbvm.com

[Q41] 多表连接
来源：http://mid.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://kfl.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://fzr.haohaochexian.top

JOIN products p ON p.id = o.product_id;
来源：http://qbb.jqgfzy.top

[Q42] 连接条件附加过滤
来源：http://ckw.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://jkc.birdmap.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kva.shanyushiyangkeji.top

[Q43] 标量子查询
来源：http://osi.sjlbkw.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hsf.haohaochexian.top

[Q44] IN 子查询
来源：http://nli.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rhq.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://xgr.hongshengwenyu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dsd.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://lgz.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gvf.tianlin.xyz

[Q47] 与平均值比较
来源：http://ypv.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gri.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://its.tianlin.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nat.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://pmm.epnwcf.com

[Q49] 更新单行
来源：http://owe.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xzf.guowangkeji.top

[Q50] 批量更新
来源：http://guq.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tnl.shuidangran.top

[Q51] 用子查询更新
来源：http://zqw.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bgu.vqdsnc.cn

[Q52] 删除指定行
来源：http://tdx.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://mnv.hongshengwenyu.top

[Q53] 按条件删除
来源：http://zcr.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tlv.iojbl.cn

[Q54] 清空表
来源：http://iku.birdmap.top

TRUNCATE TABLE logs;
来源：http://upc.haohaochexian.top

[Q55] 排名（并列占位）
来源：http://yzb.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://khk.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://qwg.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jfc.andypj.xyz

[Q57] 行号
来源：http://pin.zdqjudy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nvm.tian-w.cn

[Q58] 累计求和
来源：http://tim.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hlu.yj202588.top

[Q59] 分组内累计
来源：http://ils.yongpay.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qrm.cucudq.cn

[Q60] 取上一行 / 下一行
来源：http://iku.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sxx.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://odh.ywan-chungtsiang.top

[Q61] 移动平均
来源：http://iyh.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://toh.xziqi.cn

[Q62] 分组占比
来源：http://sga.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kog.dashuyun.cn

[Q63] 开启事务
来源：http://iet.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wko.yvedp.cn

[Q64] 提交事务
来源：http://jqc.jyoumei.cn

COMMIT;
来源：http://mbb.jqgufenzy.top

[Q65] 回滚事务
来源：http://zmt.uphjek.com

ROLLBACK;
来源：http://jkw.cashguo.top

[Q66] 行锁查询
来源：http://mty.yueranfly.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://duh.gotoacloud.top

[Q67] 设置隔离级别
来源：http://gts.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nss.gzhubu.top

[Q68] 保存点
来源：http://jwd.tianlin.xyz

SAVEPOINT sp1;
来源：http://lgr.gogol.net.cn

ROLLBACK TO sp1;
来源：http://ayg.jinqigufen.top

[Q69] 查看执行计划
来源：http://tvp.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uos.dashuyun.cn

[Q70] 更新统计信息
来源：http://ulf.nwbrower.top

ANALYZE TABLE users;
来源：http://uck.ywan-chungtsiang.top

[Q71] 查看建表语句
来源：http://wnj.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://woh.hfpthk.cn

[Q72] 查看索引
来源：http://hlj.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://sjv.sufxvd.cn

[Q73] 查看表状态
来源：http://svg.fehbvm.com

SHOW TABLE STATUS LIKE 'users';
来源：http://rnq.jqgfzy.top

[Q74] 强制使用索引
来源：http://pmj.ctjpmb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gmv.quarkkingdee.top

[Q75] 日期格式化
来源：http://dqi.dianchejie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lvx.zhaomingkeji.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rdv.smart0.xyz

[Q76] 按天统计
来源：http://nab.xziqi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tbb.shuidangran.top

[Q77] 时间加减
来源：http://ocl.gaohongyu789.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xhd.52xcode.cn

[Q78] 当前时间
来源：http://qsy.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lph.jiagoushi.top

[Q79] 字符串拼接
来源：http://cox.ctjpmb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://izk.fktsv.cn

[Q80] 字符串截取
来源：http://ckf.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mww.xinyue.icu

[Q81] 字符串替换
来源：http://mzs.xinyue.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dsf.sweek.top

[Q82] 字符长度与字节长度
来源：http://ize.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mfn.zycfv.cn

[Q83] 大小写转换
来源：http://uwm.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hgr.zhengqikj.top

[Q84] 去除首尾空格
来源：http://cob.meibo888.top

SELECT TRIM(name) FROM users;
来源：http://oij.xziqi.cn

[Q85] 数值取整
来源：http://ypl.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qsq.zhoulong.xyz

[Q86] 读取 JSON 字段
来源：http://jwn.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mri.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://tem.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xgj.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://ddj.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ofj.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uxm.9152youxi.cn

[Q89] 判断表是否存在
来源：http://vqc.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bed.haohaochexian.top

[Q90] 生成序号列
来源：http://twe.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wok.hammf.cn

================================================================================
来源：http://bhw.vqdsnc.cn

R. Bash 专题
来源：http://lrj.jinyuanbaomall.cn

================================================================================
来源：http://yds.svipenyu.cn

[R01] shebang 与严格模式
来源：http://fce.yfazqb.com

#!/usr/bin/env bash
来源：http://ykr.pengpengdd.cyou

set -euo pipefail
来源：http://gyu.pycfn.com

[R02] 变量赋值与使用
来源：http://gru.zycfv.cn

name="Tom"; echo "$name"
来源：http://dzn.chenlongwang.top

[R03] 只读变量
来源：http://gdd.zhaomingkeji.xyz

readonly PI=3.14
来源：http://xws.sysykeji.top

[R04] 位置参数
来源：http://qcp.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pbd.jyoumei.cn

[R05] 参数默认值
来源：http://dyi.jqgufenzy.top

name="${1:-default}"
来源：http://lox.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://qns.vqdsnc.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://taz.yueranfly.top

[R07] if 判断文件
来源：http://ozs.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fua.chenzaomai.com

[R08] 数值比较
来源：http://wrw.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mqb.sufxvd.cn

[R09] 字符串比较
来源：http://lsy.zhixingplan.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qso.tianlin.xyz

[R10] 正则匹配
来源：http://xtp.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wkj.xziqi.cn

[R11] case 多分支
来源：http://evx.dianchejie.cn

case "$1" in
来源：http://wzw.fehbvm.com

start) echo "启动" ;;
来源：http://lhm.guowangkeji.top

stop)  echo "停止" ;;
来源：http://rht.hesvh.cn

*)     echo "未知命令" ;;
来源：http://jmu.cqqwz.cn

esac
来源：http://zam.fzhhl.top

[R12] for 遍历文件
来源：http://vfg.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://vcp.ivvv.top

[R13] for 计数循环
来源：http://wki.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://tvg.fzhhl.top

[R14] C 风格 for
来源：http://zal.gzhubu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://imw.yongpay.top

[R15] while 逐行读文件
来源：http://crs.gotoacloud.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mey.vehdjk.com

[R16] until 等待条件
来源：http://ztv.iojbl.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mzz.shanyushiyangkeji.top

[R17] 数组定义与取值
来源：http://dvr.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://dap.epnwcf.com

[R18] 遍历数组
来源：http://rft.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ypr.zhijiandao.cn

[R19] 数组长度
来源：http://vvq.haohaochexian.top

echo "${#arr[@]}"
来源：http://jes.epnwcf.com

[R20] 关联数组（字典）
来源：http://fcn.jqgufenzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mce.birdmap.top

[R21] 字符串长度
来源：http://jqn.jqgufenzy.top

echo "${#s}"
来源：http://xxe.haohaochexian.top

[R22] 截取子串
来源：http://zby.hnxiangtu.top

echo "${s:0:5}"
来源：http://ckw.feifeiyinyue.top

[R23] 字符串替换
来源：http://cof.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cvt.cdnleiting.top

[R24] 大小写转换
来源：http://brp.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iiy.cashguo.top

[R25] 去后缀 / 去前缀
来源：http://qha.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rke.shanyushiyangtech.top

[R26] 命令替换
来源：http://kpy.yanxiufei.cn

now=$(date +%F); echo "$now"
来源：http://xxx.9152youxi.cn

[R27] 算术展开
来源：http://svu.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://err.shangyingyoupin.top

[R28] 浮点运算
来源：http://lak.daria6918.cn

echo "scale=2; 10/3" | bc
来源：http://dgp.tarul.cn

[R29] 定义函数
来源：http://uop.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://equ.tianlin.xyz

[R30] 函数返回状态码
来源：http://omz.ydzc1.top

f() { return 0; }; f || echo "失败了"
来源：http://cqs.hysaishi.cn

[R31] 局部变量
来源：http://zme.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://qij.hywenlv.cn

[R32] 参数个数校验
来源：http://yud.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qvl.cheryme.top

[R33] 捕获错误并提示行号
来源：http://ucl.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jwn.hnxiangtu.top

[R34] 退出时清理
来源：http://qzp.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nyh.zhoulong.xyz

[R35] 后台执行并等待
来源：http://grz.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iyr.zhengqikj.top

[R36] 并发执行多个任务
来源：http://ocj.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://umz.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://fuy.bbcook.cn

files=$(ls -1)
来源：http://tkt.yuanzhike.top

[R38] 管道串联
来源：http://tav.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://qts.cheryme.top

[R39] 重定向标准输出与错误
来源：http://mkw.jqgufenzy.top

cmd > out.log 2>&1
来源：http://abn.hnqzz.top

[R40] 追加写日志
来源：http://xiz.fzhhl.top

echo "log" >> out.log
来源：http://kgc.zhiwuduotai.top

[R41] 丢弃输出
来源：http://ujh.vehdjk.com

cmd >/dev/null 2>&1
来源：http://ezy.jinghuilouyu.cn

[R42] 输入重定向
来源：http://tsl.shangyingyoupin.top

wc -l < a.txt
来源：http://ecv.hammf.cn

[R43] 按名字查找文件
来源：http://hyp.vehdjk.com

find . -name "*.log" -type f
来源：http://syd.hysaishi.cn

[R44] 按修改时间查找
来源：http://yry.mhx1999.top

find . -mtime -7 -type f
来源：http://ntf.jqgufenzy.top

[R45] 批量删除
来源：http://wku.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://xfs.shuidangran.top

[R46] 递归替换文件内容
来源：http://mel.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nio.sjlbkw.cn

[R47] sed 单行替换
来源：http://jas.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pjy.dianchejie.cn

[R48] awk 取指定列
来源：http://qnv.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://qhs.zhongyouzk.top

[R49] awk 带条件
来源：http://jgb.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sey.zdqjudy.top

[R50] awk 求和
来源：http://qkg.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://szm.uphjek.com

[R51] 排序去重取前几
来源：http://gog.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://bcn.zycfv.cn

[R52] 统计行数
来源：http://ppc.gogol.net.cn

wc -l a.txt
来源：http://mde.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://lwy.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mhc.xuanzx.com

[R54] 比较两个文件
来源：http://plv.sufxvd.cn

diff a.txt b.txt
来源：http://foe.birdmap.top

[R55] 压缩与解压
来源：http://zah.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tgw.tarul.cn

[R56] 远程拷贝
来源：http://guk.nanxinkj.top

scp file user@host:/path/
来源：http://ygm.dashuyun.cn

[R57] 远程执行命令
来源：http://ums.andypj.xyz

ssh user@host 'uptime'
来源：http://tkr.fktsv.cn

[R58] 下载文件
来源：http://rzt.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://upq.sufxvd.cn

[R59] 发 POST JSON
来源：http://yyh.tian-w.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sdl.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://nwg.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cdf.cheryme.top

[R61] 磁盘占用
来源：http://sbf.pengpengdd.cyou

df -h;  du -sh *
来源：http://cwu.iojbl.cn

[R62] 找最占空间的文件
来源：http://oul.cashguo.top

du -ah . | sort -rh | head -10
来源：http://zrz.zhixingplan.top

[R63] 内存与进程
来源：http://oqk.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://jlg.sweek.top

[R64] 结束进程
来源：http://wks.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://ywh.wangshuangyany.cn

[R65] 查看端口占用
来源：http://pnx.haohaochexian.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yyf.yanxiufei.cn

[R66] 定时任务
来源：http://kca.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://vql.jiagoushi.top

[R67] 生成随机十六进制串
来源：http://wru.316326.xyz

openssl rand -hex 16
来源：http://awx.snrcjt.cn

[R68] 计算文件校验值
来源：http://lfh.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ifn.cheryme.top

[R69] 生成随机密码
来源：http://vtq.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://qxe.sufxvd.cn

[R70] 时间戳与互转
来源：http://dta.yj20258.top

date +%s;  date -d @1700000000
来源：http://hki.zdbjq.cn

[R71] 日期格式化
来源：http://bfv.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://hbb.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://bqu.ydjk.org.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jmi.pengpengdd.cyou

[R73] 分割大日志
来源：http://tlq.ehwqpu.com


<!-- 参考信息 -->