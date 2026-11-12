代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rkj.shangyingyoupin.top

[Q28] 求和与平均
来源：http://jbf.xinyue.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xsp.yfazqb.com

[Q29] 最大最小值
来源：http://xpw.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ifi.tian-w.cn

[Q30] 分组统计
来源：http://gpu.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ezz.hywenlv.cn

[Q31] 分组后过滤
来源：http://nae.zhixingplan.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hom.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://jgj.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kry.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mrd.shangyingyoupin.top

[Q33] 多列分组
来源：http://rrj.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dzl.9152youxi.cn

[Q34] 每组取第一条
来源：http://tgj.pengpengdd.cyou

SELECT * FROM (
来源：http://nez.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sup.sufxvd.cn

) t WHERE rn = 1;
来源：http://vsc.xylfe.cn

[Q35] 内连接
来源：http://ieh.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gxs.tanke756.top

[Q36] 左连接
来源：http://flz.jlsjyb.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ttb.jyoumei.cn

[Q37] 右连接
来源：http://zgx.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mfu.316326.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://adb.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eqp.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://uct.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qbx.zdbjq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://joq.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://jaq.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://suo.sxryk.cn

[Q41] 多表连接
来源：http://zkm.zhiwuduotai.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fnd.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://eeg.chenzaomai.com

JOIN products p ON p.id = o.product_id;
来源：http://dgz.haohaochexian.top

[Q42] 连接条件附加过滤
来源：http://kwu.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u
来源：http://pqf.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://whi.hesvh.cn

[Q43] 标量子查询
来源：http://hqm.ctjpmb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kik.dashuyun.cn

[Q44] IN 子查询
来源：http://joo.aizwys.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://smy.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://rcd.zhengqikj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nmb.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://diz.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gtk.yuanzhike.top

[Q47] 与平均值比较
来源：http://xde.fanxiaobao.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xig.jinqigfzy.top

[Q48] CTE 公用表表达式
来源：http://xzg.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ehf.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://afa.chenlongwang.top

[Q49] 更新单行
来源：http://vnd.vehdjk.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://awd.yj20258.top

[Q50] 批量更新
来源：http://moy.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mqo.hfpthk.cn

[Q51] 用子查询更新
来源：http://dwu.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gqv.hysaishi.cn

[Q52] 删除指定行
来源：http://kab.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://jlj.chenjidiqi.icu

[Q53] 按条件删除
来源：http://wen.dianchejie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iuc.gogol.net.cn

[Q54] 清空表
来源：http://dzk.pycfn.com

TRUNCATE TABLE logs;
来源：http://jrh.svipenyu.cn

[Q55] 排名（并列占位）
来源：http://hra.sweek.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://joi.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://crz.dashuyun.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bnt.andypj.xyz

[Q57] 行号
来源：http://gsp.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ixl.zhixingplan.top

[Q58] 累计求和
来源：http://kjd.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xif.shanyushiyangkeji.top

[Q59] 分组内累计
来源：http://nwz.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nss.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://qlj.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://awo.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qvw.hysaishi.cn

[Q61] 移动平均
来源：http://ifw.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://grw.pycfn.com

[Q62] 分组占比
来源：http://ofd.jiagoushi.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nel.smart0.xyz

[Q63] 开启事务
来源：http://cim.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zmy.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://ytm.jinqigfzy.top

COMMIT;
来源：http://hgt.sweek.top

[Q65] 回滚事务
来源：http://sfh.cashguo.top

ROLLBACK;
来源：http://whm.fehbvm.com

[Q66] 行锁查询
来源：http://exk.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gzu.ydzc1.top

[Q67] 设置隔离级别
来源：http://mes.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uuo.bbcook.cn

[Q68] 保存点
来源：http://cdi.xuanzx.com

SAVEPOINT sp1;
来源：http://fql.snrcjt.cn

ROLLBACK TO sp1;
来源：http://zzx.ivvv.top

[Q69] 查看执行计划
来源：http://nex.andypj.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://umy.nanxuanxn.top

[Q70] 更新统计信息
来源：http://lbj.nwbrower.top

ANALYZE TABLE users;
来源：http://dcl.gogol.net.cn

[Q71] 查看建表语句
来源：http://ndx.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://evn.andypj.xyz

[Q72] 查看索引
来源：http://mwe.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://gfa.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://qlf.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fzd.bbcook.cn

[Q74] 强制使用索引
来源：http://kkh.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bit.havefunace.top

[Q75] 日期格式化
来源：http://usc.yongpay.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://epr.xziqi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://afc.snrcjt.cn

[Q76] 按天统计
来源：http://zif.hcnkem.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uaf.zhiwuduotai.top

[Q77] 时间加减
来源：http://vge.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eep.bbcook.cn

[Q78] 当前时间
来源：http://zvh.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://llf.yfazqb.com

[Q79] 字符串拼接
来源：http://cof.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vpl.kuanghao11.cn

[Q80] 字符串截取
来源：http://jid.fehbvm.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mdw.xinyue.icu

[Q81] 字符串替换
来源：http://igo.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zwx.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://oop.zhiwuduotai.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pzu.feifeiyinyue.top

[Q83] 大小写转换
来源：http://iam.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bku.ybcxt.top

[Q84] 去除首尾空格
来源：http://zzr.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://vie.tianlin.xyz

[Q85] 数值取整
来源：http://mvk.zdbjq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://utj.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://gtm.hongshengwenyu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qlz.yj202588.top

[Q87] JSON 字段做条件
来源：http://dgz.cashguo.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tlh.jinyuanbaomall.cn

[Q88] 行转列（条件聚合）
来源：http://xon.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mac.tianlin.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://isq.guannengcc.top

[Q89] 判断表是否存在
来源：http://mhq.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pkx.0kj1m.cn

[Q90] 生成序号列
来源：http://lrw.iojbl.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://okb.zdqjudy.top

================================================================================
来源：http://fbg.shzxlz.cn

R. Bash 专题
来源：http://php.jqgfzy.top

================================================================================
来源：http://dho.nanxinkj.top

[R01] shebang 与严格模式
来源：http://sou.xziqi.cn

#!/usr/bin/env bash
来源：http://jlv.gogol.net.cn

set -euo pipefail
来源：http://puo.hywenlv.cn

[R02] 变量赋值与使用
来源：http://ikb.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://ize.zhaomingkeji.xyz

[R03] 只读变量
来源：http://egd.dashuyun.cn

readonly PI=3.14
来源：http://zvn.meibo888.top

[R04] 位置参数
来源：http://tkd.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cvc.sysykeji.top

[R05] 参数默认值
来源：http://gyl.andypj.xyz

name="${1:-default}"
来源：http://oop.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://ybt.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rng.pycfn.com

[R07] if 判断文件
来源：http://yll.chenzaomai.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zib.zhiwuduotai.top

[R08] 数值比较
来源：http://cns.jianghu66.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yrr.hongshengwenyu.top

[R09] 字符串比较
来源：http://wmp.hcnkem.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ckl.kuanghao11.cn

[R10] 正则匹配
来源：http://gwa.xylfe.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hju.andypj.xyz

[R11] case 多分支
来源：http://uez.xziqi.cn

case "$1" in
来源：http://koq.hnqzz.top

start) echo "启动" ;;
来源：http://ehz.tarul.cn

stop)  echo "停止" ;;
来源：http://sqx.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://ewn.bbcook.cn

esac
来源：http://dfs.gzhubu.top

[R12] for 遍历文件
来源：http://fpe.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://ksh.ydzc1.top

[R13] for 计数循环
来源：http://mas.52xcode.cn

for i in {1..10}; do echo "$i"; done
来源：http://uxq.havefunace.top

[R14] C 风格 for
来源：http://dzd.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xqm.ctjpmb.com

[R15] while 逐行读文件
来源：http://qmc.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lmg.tianlin.xyz

[R16] until 等待条件
来源：http://ipz.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ham.fengsongda.top

[R17] 数组定义与取值
来源：http://xrp.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://dzr.zhaomingkeji.xyz

[R18] 遍历数组
来源：http://etm.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qew.zdbjq.cn

[R19] 数组长度
来源：http://yvw.vqdsnc.cn

echo "${#arr[@]}"
来源：http://nuw.cdnleiting.top

[R20] 关联数组（字典）
来源：http://grl.gogol.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vun.bbcook.cn

[R21] 字符串长度
来源：http://iim.shanyushiyangkeji.top

echo "${#s}"
来源：http://gun.ydzc1.top

[R22] 截取子串
来源：http://kfv.zhixingplan.top

echo "${s:0:5}"
来源：http://yki.svipenyu.cn

[R23] 字符串替换
来源：http://rtn.dianchejie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wpq.zhijiandao.cn

[R24] 大小写转换
来源：http://prw.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://lrn.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://bif.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ahd.haohaochexian.top

[R26] 命令替换
来源：http://qsc.ydjk.org.cn

now=$(date +%F); echo "$now"
来源：http://xke.hnxiangtu.top

[R27] 算术展开
来源：http://edu.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://ncu.sweek.top

[R28] 浮点运算
来源：http://prs.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://ndd.nanxinkj.top

[R29] 定义函数
来源：http://aqo.fengsongda.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yyd.nanxuanxn.top

[R30] 函数返回状态码
来源：http://asl.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://dcw.shanyushiyangkeji.top

[R31] 局部变量
来源：http://wkl.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://hoa.quarkkingdee.top

[R32] 参数个数校验
来源：http://tmb.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vuj.yongpay.top

[R33] 捕获错误并提示行号
来源：http://hty.jiagoushi.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gmo.andypj.xyz

[R34] 退出时清理
来源：http://xzx.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kaf.shzxlz.cn

[R35] 后台执行并等待
来源：http://hzb.tanke756.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gai.sxryk.cn

[R36] 并发执行多个任务
来源：http://xhw.ehwqpu.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kaw.hywenlv.cn

[R37] 把输出赋给变量
来源：http://fjw.redwolf501.top

files=$(ls -1)
来源：http://yek.xuanzx.com

[R38] 管道串联
来源：http://hzm.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://rbs.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://eig.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://ddz.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://gjo.hcnkem.com

echo "log" >> out.log
来源：http://jdm.jqgufenzy.top

[R41] 丢弃输出
来源：http://xmc.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://usr.tanke756.top

[R42] 输入重定向
来源：http://uwb.jinqigufen.top

wc -l < a.txt
来源：http://tnt.9152youxi.cn

[R43] 按名字查找文件
来源：http://vne.nanxuanxn.top

find . -name "*.log" -type f
来源：http://lmn.tarul.cn

[R44] 按修改时间查找
来源：http://gcu.jqgufenzy.top

find . -mtime -7 -type f
来源：http://zck.iojbl.cn

[R45] 批量删除
来源：http://yjq.epnwcf.com

find . -name "*.tmp" -delete
来源：http://rwy.xziqi.cn

[R46] 递归替换文件内容
来源：http://vvj.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://whc.ybcxt.top

[R47] sed 单行替换
来源：http://ezm.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://rlb.sysykeji.top

[R48] awk 取指定列
来源：http://zbq.shzxlz.cn

awk '{print $1, $3}' a.txt
来源：http://jtf.nanxinkj.top

[R49] awk 带条件
来源：http://hjs.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ljp.jyoumei.cn

[R50] awk 求和
来源：http://yed.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://jgn.havefunace.top

[R51] 排序去重取前几
来源：http://imn.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zih.gogol.net.cn

[R52] 统计行数
来源：http://ojf.jlsjyb.cn

wc -l a.txt
来源：http://zyi.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://ulj.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://trv.svipenyu.cn

[R54] 比较两个文件
来源：http://vaw.yanxiufei.cn

diff a.txt b.txt
来源：http://eud.wangshuangyany.cn

[R55] 压缩与解压
来源：http://kld.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pew.jianghu66.top

[R56] 远程拷贝
来源：http://rzj.ywan-chungtsiang.top

scp file user@host:/path/
来源：http://qwg.nwbrower.top

[R57] 远程执行命令
来源：http://uxd.ivvv.top

ssh user@host 'uptime'
来源：http://dki.dashuyun.cn

[R58] 下载文件
来源：http://thh.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ejn.zhixingplan.top

[R59] 发 POST JSON
来源：http://ipy.hammf.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oiw.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://fqz.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kfx.yvedp.cn

[R61] 磁盘占用
来源：http://qpz.zhengqikj.top

df -h;  du -sh *
来源：http://ycf.bbcook.cn

[R62] 找最占空间的文件
来源：http://woj.jinqigufen.top

du -ah . | sort -rh | head -10
来源：http://cru.yfazqb.com

[R63] 内存与进程
来源：http://uia.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://fyy.zhengqikj.top

[R64] 结束进程
来源：http://zqu.jianghu66.top

kill -9 $(pgrep -f app.py)
来源：http://ubh.mhx1999.top

[R65] 查看端口占用
来源：http://lcx.shanyushiyangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qbl.jinqigufen.top

[R66] 定时任务
来源：http://kgo.sxryk.cn

crontab -e;  crontab -l
来源：http://afl.ydzc1.top

[R67] 生成随机十六进制串
来源：http://jhj.hysaishi.cn

openssl rand -hex 16
来源：http://vew.zhixingplan.top

[R68] 计算文件校验值
来源：http://tea.zhixingplan.top

sha256sum a.txt;  md5sum a.txt
来源：http://zii.ehwqpu.com

[R69] 生成随机密码
来源：http://ipj.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://vpd.jlsjyb.cn

[R70] 时间戳与互转
来源：http://qvd.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://bev.bbcook.cn

[R71] 日期格式化
来源：http://cas.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xzn.sysykeji.top

[R72] 等待端口就绪
来源：http://ovk.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://qpt.pengpengdd.cyou

[R73] 分割大日志
来源：http://san.guannengcc.top

split -l 1000 big.log part_
来源：http://ylg.yuanzhike.top

[R74] 批量重命名
来源：http://gwx.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cgn.zhiwuduotai.top

[R75] 导出环境变量
来源：http://hle.ctjpmb.com

export PATH="$HOME/bin:$PATH"
来源：http://oiu.mhx1999.top

[R76] 使用临时文件
来源：http://lly.svipenyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zgt.jiagoushi.top

[R77] 读取用户输入
来源：http://mkl.cdnleiting.top


<!-- 参考信息 -->