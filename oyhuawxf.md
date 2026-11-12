代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bfe.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://obh.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://agm.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xjr.jlsjyb.cn

[Q33] 多列分组
来源：http://yjc.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bhd.fengsongda.top

[Q34] 每组取第一条
来源：http://nge.hfpthk.cn

SELECT * FROM (
来源：http://kbr.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wqs.zhoulong.xyz

) t WHERE rn = 1;
来源：http://bwa.tarul.cn

[Q35] 内连接
来源：http://slq.uphjek.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tca.hesvh.cn

[Q36] 左连接
来源：http://lke.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zig.jinqigfzy.top

[Q37] 右连接
来源：http://xoq.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ysf.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://wdf.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bwg.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://lyb.tanke756.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nyi.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kss.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://atr.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://voi.hongshengwenyu.top

[Q41] 多表连接
来源：http://uge.zhixingplan.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sip.tanke756.top

JOIN users u ON u.id = o.user_id
来源：http://dvx.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://uzq.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://hkn.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://axc.vqdsnc.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aqe.xuetiantiany.cn

[Q43] 标量子查询
来源：http://lyv.zycfv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kfv.quarkkingdee.top

[Q44] IN 子查询
来源：http://wtr.0kj1m.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ezy.ydjk.org.cn

[Q45] EXISTS 判断存在
来源：http://kji.c1oappe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wce.bbcook.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xtj.bbcook.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zfb.epnwcf.com

[Q47] 与平均值比较
来源：http://jkx.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rrd.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://kww.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zom.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://bod.ehwqpu.com

[Q49] 更新单行
来源：http://sbk.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wfm.kuanghao11.cn

[Q50] 批量更新
来源：http://ltn.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uja.tarul.cn

[Q51] 用子查询更新
来源：http://leg.aizwys.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nwj.jlsjyb.cn

[Q52] 删除指定行
来源：http://pur.zhixingplan.top

DELETE FROM users WHERE id = 10;
来源：http://lmi.shzxlz.cn

[Q53] 按条件删除
来源：http://iwz.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://khb.xingfuxueyuan.xyz

[Q54] 清空表
来源：http://ixu.jinghuilouyu.cn

TRUNCATE TABLE logs;
来源：http://djx.xuanzx.com

[Q55] 排名（并列占位）
来源：http://hno.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dux.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://jdt.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hjr.epnwcf.com

[Q57] 行号
来源：http://auz.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vxg.jianghu66.top

[Q58] 累计求和
来源：http://qgd.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kks.sxryk.cn

[Q59] 分组内累计
来源：http://zzb.daria6918.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wvq.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://aki.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ujz.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tzt.chenzaomai.com

[Q61] 移动平均
来源：http://oyb.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jcv.yueranfly.top

[Q62] 分组占比
来源：http://yab.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fsl.yj20258.top

[Q63] 开启事务
来源：http://hix.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://orr.dashuyun.cn

[Q64] 提交事务
来源：http://hgm.ydzc1.top

COMMIT;
来源：http://pfr.ivvv.top

[Q65] 回滚事务
来源：http://vzz.nanxinkj.top

ROLLBACK;
来源：http://ycg.dashuyun.cn

[Q66] 行锁查询
来源：http://bwl.daxiang520.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gri.yueranfly.top

[Q67] 设置隔离级别
来源：http://sbb.chenzaomai.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://exg.shanyushiyangkeji.top

[Q68] 保存点
来源：http://yfp.yj20258888.top

SAVEPOINT sp1;
来源：http://niv.bjfxy.top

ROLLBACK TO sp1;
来源：http://cjs.hnqzz.top

[Q69] 查看执行计划
来源：http://qsg.yfazqb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uyj.aibaodan.cn

[Q70] 更新统计信息
来源：http://owj.jinghuilouyu.cn

ANALYZE TABLE users;
来源：http://sbi.yangfankeji.com

[Q71] 查看建表语句
来源：http://erz.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jlo.zhixingplan.top

[Q72] 查看索引
来源：http://dlx.svipenyu.cn

SHOW INDEX FROM users;
来源：http://qtk.zdqjudy.top

[Q73] 查看表状态
来源：http://eoz.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ihg.vqdsnc.cn

[Q74] 强制使用索引
来源：http://ymk.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dvu.0kj1m.cn

[Q75] 日期格式化
来源：http://wxx.havefunace.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wxb.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ldh.0kj1m.cn

[Q76] 按天统计
来源：http://spu.ppjwa.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ljm.fehbvm.com

[Q77] 时间加减
来源：http://rus.bjfxy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yta.daxiang520.top

[Q78] 当前时间
来源：http://zcx.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xfh.gotoacloud.top

[Q79] 字符串拼接
来源：http://xvl.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eqe.guannengcc.top

[Q80] 字符串截取
来源：http://wle.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://urf.chenzaomai.com

[Q81] 字符串替换
来源：http://emd.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fvt.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://xqz.ctjpmb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lnf.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://hhp.jinghuilouyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://roj.sweek.top

[Q84] 去除首尾空格
来源：http://yfd.chenzaomai.com

SELECT TRIM(name) FROM users;
来源：http://ita.xziqi.cn

[Q85] 数值取整
来源：http://qdr.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ssg.zhijiandao.cn

[Q86] 读取 JSON 字段
来源：http://pfn.yuanzhike.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://czf.xylfe.cn

[Q87] JSON 字段做条件
来源：http://oiz.fengsongda.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hgu.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://brq.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qny.chenjidiqi.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fqi.jyoumei.cn

[Q89] 判断表是否存在
来源：http://zkm.chenlongwang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vod.yanxiufei.cn

[Q90] 生成序号列
来源：http://nwj.jinqigfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://can.zycfv.cn

================================================================================
来源：http://jls.zdbjq.cn

R. Bash 专题
来源：http://tjb.nanxuanxn.top

================================================================================
来源：http://ziw.zhoulong.xyz

[R01] shebang 与严格模式
来源：http://ihk.ehwqpu.com

#!/usr/bin/env bash
来源：http://kuy.zhaomingkeji.xyz

set -euo pipefail
来源：http://kme.jqgfzy.top

[R02] 变量赋值与使用
来源：http://rgd.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://edw.pycfn.com

[R03] 只读变量
来源：http://mdj.zdqjudy.top

readonly PI=3.14
来源：http://jtl.guowangkeji.top

[R04] 位置参数
来源：http://ujz.bjfxy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qcp.c1oappe.top

[R05] 参数默认值
来源：http://qzo.nanxuanxn.top

name="${1:-default}"
来源：http://xko.nanxinkj.top

[R06] 判断命令是否存在
来源：http://uad.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fss.xinyue.icu

[R07] if 判断文件
来源：http://iag.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rzw.shanyushiyangkeji.top

[R08] 数值比较
来源：http://cnm.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ilq.mhx1999.top

[R09] 字符串比较
来源：http://foq.tarul.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nls.hnxiangtu.top

[R10] 正则匹配
来源：http://ibr.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yqg.chenzaomai.com

[R11] case 多分支
来源：http://alb.yuxming.cn

case "$1" in
来源：http://mpt.zhixingplan.top

start) echo "启动" ;;
来源：http://yse.gogol.net.cn

stop)  echo "停止" ;;
来源：http://ahr.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://ujp.fengsongda.top

esac
来源：http://rjr.jqgufenzy.top

[R12] for 遍历文件
来源：http://qhd.c1oappe.top

for f in *.txt; do echo "$f"; done
来源：http://uqt.sufxvd.cn

[R13] for 计数循环
来源：http://plm.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://brk.xuetiantiany.cn

[R14] C 风格 for
来源：http://gzd.zhengqikj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ncg.iojbl.cn

[R15] while 逐行读文件
来源：http://soy.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rdw.yvedp.cn

[R16] until 等待条件
来源：http://ecv.pycfn.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jao.yueranfly.top

[R17] 数组定义与取值
来源：http://est.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://mnf.zhijiandao.cn

[R18] 遍历数组
来源：http://ngw.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gsc.redwolf501.top

[R19] 数组长度
来源：http://ztg.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://dmy.yj202588.top

[R20] 关联数组（字典）
来源：http://zbx.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jfm.jinqigfzy.top

[R21] 字符串长度
来源：http://hyg.jiagoushi.top

echo "${#s}"
来源：http://bas.chenzaomai.com

[R22] 截取子串
来源：http://zie.xziqi.cn

echo "${s:0:5}"
来源：http://jnf.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://uwx.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kuh.hywenlv.cn

[R24] 大小写转换
来源：http://mai.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://moc.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://lul.epnwcf.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://jnd.yongpay.top

[R26] 命令替换
来源：http://ccm.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://uke.jinqigfzy.top

[R27] 算术展开
来源：http://qww.hesvh.cn

echo $((1 + 2 * 3))
来源：http://mtg.shzxlz.cn

[R28] 浮点运算
来源：http://ean.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://ftu.jqgufenzy.top

[R29] 定义函数
来源：http://kpc.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kwb.kuanghao11.cn

[R30] 函数返回状态码
来源：http://ojf.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://kdi.jlsjyb.cn

[R31] 局部变量
来源：http://qkn.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://cra.gzhubu.top

[R32] 参数个数校验
来源：http://ekg.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bry.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://otp.bjfxy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bag.nwbrower.top

[R34] 退出时清理
来源：http://mup.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://irn.shuidangran.top

[R35] 后台执行并等待
来源：http://pbw.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kxy.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://jkt.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pho.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://rbl.hfpthk.cn

files=$(ls -1)
来源：http://xzy.nanxinkj.top

[R38] 管道串联
来源：http://org.fzhhl.top

cat a.txt | grep -i error | wc -l
来源：http://zdv.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://jtb.ydjk.org.cn

cmd > out.log 2>&1
来源：http://wgo.hywenlv.cn

[R40] 追加写日志
来源：http://zyd.fktsv.cn

echo "log" >> out.log
来源：http://dbw.fzhhl.top

[R41] 丢弃输出
来源：http://ifp.epnwcf.com

cmd >/dev/null 2>&1
来源：http://rxd.hysaishi.cn

[R42] 输入重定向
来源：http://qxu.zhoulong.xyz

wc -l < a.txt
来源：http://qwh.zhengqikj.top

[R43] 按名字查找文件
来源：http://uwa.kuanghao11.cn

find . -name "*.log" -type f
来源：http://qab.nwbrower.top

[R44] 按修改时间查找
来源：http://idf.zdqjudy.top

find . -mtime -7 -type f
来源：http://krx.zhaomingkeji.xyz

[R45] 批量删除
来源：http://rbx.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://nro.cheryme.top

[R46] 递归替换文件内容
来源：http://fik.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gan.gotoacloud.top

[R47] sed 单行替换
来源：http://ysj.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://sbm.cqqwz.cn

[R48] awk 取指定列
来源：http://qpd.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://mdd.aibaodan.cn

[R49] awk 带条件
来源：http://oke.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jhm.guannengcc.top

[R50] awk 求和
来源：http://uvs.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://cqi.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://lpe.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cwm.ehwqpu.com

[R52] 统计行数
来源：http://sft.tian-w.cn

wc -l a.txt
来源：http://mhv.jinqigufen.top

[R53] 查看文件头与实时尾
来源：http://ynt.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jbw.dianchejie.cn

[R54] 比较两个文件
来源：http://drd.ppjwa.cn

diff a.txt b.txt
来源：http://iif.hammf.cn

[R55] 压缩与解压
来源：http://zql.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vwm.iojbl.cn

[R56] 远程拷贝
来源：http://odh.jlsjyb.cn

scp file user@host:/path/
来源：http://nfp.pengpengdd.cyou

[R57] 远程执行命令
来源：http://lza.hysaishi.cn

ssh user@host 'uptime'
来源：http://dit.pengpengdd.cyou

[R58] 下载文件
来源：http://wux.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pqy.wangdashe.top

[R59] 发 POST JSON
来源：http://cos.bjfxy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ehl.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://lzb.tian-w.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oeo.shuidangran.top

[R61] 磁盘占用
来源：http://zrl.ydzc1.top

df -h;  du -sh *
来源：http://knu.bbcook.cn

[R62] 找最占空间的文件
来源：http://mrw.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://ihi.yueranfly.top

[R63] 内存与进程
来源：http://ztk.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://acz.shzxlz.cn

[R64] 结束进程
来源：http://dyo.feifeiyinyue.top

kill -9 $(pgrep -f app.py)
来源：http://zdx.jianghu66.top

[R65] 查看端口占用
来源：http://nnt.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ciy.c1oappe.top

[R66] 定时任务
来源：http://moi.zhijiandao.cn

crontab -e;  crontab -l
来源：http://mqg.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://vrq.xinyue.icu

openssl rand -hex 16
来源：http://rjh.tarul.cn

[R68] 计算文件校验值
来源：http://aiv.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://mce.havefunace.top

[R69] 生成随机密码
来源：http://weu.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://xvx.quarkkingdee.top

[R70] 时间戳与互转
来源：http://qgr.epnwcf.com

date +%s;  date -d @1700000000
来源：http://ooh.0kj1m.cn

[R71] 日期格式化
来源：http://xuj.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://egg.zhijiandao.cn

[R72] 等待端口就绪
来源：http://vgb.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yth.yuanzhike.top

[R73] 分割大日志
来源：http://owr.zycfv.cn

split -l 1000 big.log part_
来源：http://bjg.kuanghao11.cn

[R74] 批量重命名
来源：http://zxu.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tee.yj20258888.top

[R75] 导出环境变量
来源：http://hec.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://hre.jinqigfzy.top

[R76] 使用临时文件
来源：http://iri.yueranfly.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dml.0kj1m.cn

[R77] 读取用户输入
来源：http://xdc.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://eii.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://hwd.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://roa.wangdashe.top

[R79] 解析命令行选项
来源：http://luq.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wur.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://xcp.ehwqpu.com

time ./run.sh
来源：http://azq.yueranfly.top

================================================================================
来源：http://rrd.tanke756.top


<!-- 参考信息 -->