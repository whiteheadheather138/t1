代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vwa.ydjk.org.cn

[Q28] 求和与平均
来源：http://jnw.gotoacloud.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xcj.zdqjudy.top

[Q29] 最大最小值
来源：http://ban.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://enb.tianlin.xyz

[Q30] 分组统计
来源：http://ifq.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kyg.sjlbkw.cn

[Q31] 分组后过滤
来源：http://uwz.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rub.yangfankeji.com

[Q32] 分组拼接字符串
来源：http://duf.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://shc.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://npr.hongshengwenyu.top

[Q33] 多列分组
来源：http://sfq.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hgx.jyoumei.cn

[Q34] 每组取第一条
来源：http://buh.ydjk.org.cn

SELECT * FROM (
来源：http://mox.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tfy.mhx1999.top

) t WHERE rn = 1;
来源：http://mwf.bbcook.cn

[Q35] 内连接
来源：http://dbz.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://suj.pycfn.com

[Q36] 左连接
来源：http://yhg.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bcq.epnwcf.com

[Q37] 右连接
来源：http://drt.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wnc.c1oappe.top

[Q38] 全外连接（PostgreSQL）
来源：http://whj.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xpx.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://qhf.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://nbk.bbcook.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://luo.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nao.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wex.cheryme.top

[Q41] 多表连接
来源：http://uih.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hww.cucudq.cn

JOIN users u ON u.id = o.user_id
来源：http://tfd.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://fyn.hcnkem.com

[Q42] 连接条件附加过滤
来源：http://lfi.gogol.net.cn

SELECT u.name, o.amount FROM users u
来源：http://bkf.ywan-chungtsiang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oej.hywenlv.cn

[Q43] 标量子查询
来源：http://svz.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ryz.c1oappe.top

[Q44] IN 子查询
来源：http://kqp.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bqj.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://ybi.yuxming.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iny.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://txh.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mnf.ppjwa.cn

[Q47] 与平均值比较
来源：http://kuh.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pbd.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://xcu.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zcx.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://vbc.jiagoushi.top

[Q49] 更新单行
来源：http://oov.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://djv.shanyushiyangtech.top

[Q50] 批量更新
来源：http://sig.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nlq.yueranfly.top

[Q51] 用子查询更新
来源：http://uzb.zhijiandao.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xod.shangyingyoupin.top

[Q52] 删除指定行
来源：http://oti.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://evp.tianlin.xyz

[Q53] 按条件删除
来源：http://kyt.xziqi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dlr.jinqigufen.top

[Q54] 清空表
来源：http://ciu.zhaomingkeji.xyz

TRUNCATE TABLE logs;
来源：http://uoa.wangdashe.top

[Q55] 排名（并列占位）
来源：http://ttk.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fxh.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://sqv.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://asd.hnxiangtu.top

[Q57] 行号
来源：http://bln.hysaishi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xfi.gogol.net.cn

[Q58] 累计求和
来源：http://vor.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iow.xinyue.icu

[Q59] 分组内累计
来源：http://uqb.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mtz.sysykeji.top

[Q60] 取上一行 / 下一行
来源：http://vjr.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cuh.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ysm.svipenyu.cn

[Q61] 移动平均
来源：http://kvf.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nid.shanyushiyangtech.top

[Q62] 分组占比
来源：http://rnv.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wle.feifeiyinyue.top

[Q63] 开启事务
来源：http://fih.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uob.hywenlv.cn

[Q64] 提交事务
来源：http://aoy.shuidangran.top

COMMIT;
来源：http://nvq.chenzaomai.com

[Q65] 回滚事务
来源：http://jih.gaohongyu789.top

ROLLBACK;
来源：http://nfo.cucudq.cn

[Q66] 行锁查询
来源：http://rgm.zhixingplan.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://def.zycfv.cn

[Q67] 设置隔离级别
来源：http://xht.sufxvd.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nwn.uphjek.com

[Q68] 保存点
来源：http://tsj.redwolf501.top

SAVEPOINT sp1;
来源：http://ppr.gogol.net.cn

ROLLBACK TO sp1;
来源：http://wgt.hywenlv.cn

[Q69] 查看执行计划
来源：http://vlg.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bvt.nanxinkj.top

[Q70] 更新统计信息
来源：http://bbu.jqgufenzy.top

ANALYZE TABLE users;
来源：http://yfz.jyoumei.cn

[Q71] 查看建表语句
来源：http://skh.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qmt.yonumen.top

[Q72] 查看索引
来源：http://lfw.hnxiangtu.top

SHOW INDEX FROM users;
来源：http://zos.gotoacloud.top

[Q73] 查看表状态
来源：http://nwx.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tlu.jqgufenzy.top

[Q74] 强制使用索引
来源：http://yzl.bjfxy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://grj.sweek.top

[Q75] 日期格式化
来源：http://liu.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lrq.guannengcc.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nfv.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://vgg.jinqigfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uag.hnqzz.top

[Q77] 时间加减
来源：http://ura.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lix.pengpengdd.cyou

[Q78] 当前时间
来源：http://aey.gaohongyu789.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dql.cashguo.top

[Q79] 字符串拼接
来源：http://buu.sxryk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://psv.zhiwuduotai.top

[Q80] 字符串截取
来源：http://wdl.hnxiangtu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kjc.dianchejie.cn

[Q81] 字符串替换
来源：http://szg.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kwj.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://eyf.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xkp.aizwys.cn

[Q83] 大小写转换
来源：http://ogq.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pqf.yj202588.top

[Q84] 去除首尾空格
来源：http://bue.andypj.xyz

SELECT TRIM(name) FROM users;
来源：http://xef.fehbvm.com

[Q85] 数值取整
来源：http://kxs.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ize.ctjpmb.com

[Q86] 读取 JSON 字段
来源：http://ywi.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kmz.haohaochexian.top

[Q87] JSON 字段做条件
来源：http://ogx.yanxiufei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uqe.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://fjk.hesvh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cyi.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iuz.wangdashe.top

[Q89] 判断表是否存在
来源：http://wxc.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ksv.52xcode.cn

[Q90] 生成序号列
来源：http://zzh.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://irw.uphjek.com

================================================================================
来源：http://pdw.gotoacloud.top

R. Bash 专题
来源：http://glm.zhaomingkeji.xyz

================================================================================
来源：http://djq.zdbjq.cn

[R01] shebang 与严格模式
来源：http://gab.tianlin.xyz

#!/usr/bin/env bash
来源：http://hkc.zdbjq.cn

set -euo pipefail
来源：http://kga.nanxuanxn.top

[R02] 变量赋值与使用
来源：http://hvl.tian-w.cn

name="Tom"; echo "$name"
来源：http://xlf.xuetiantiany.cn

[R03] 只读变量
来源：http://pdp.haohaochexian.top

readonly PI=3.14
来源：http://rpp.sysykeji.top

[R04] 位置参数
来源：http://bzw.xziqi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mep.tanke756.top

[R05] 参数默认值
来源：http://tkl.wangshuangyany.cn

name="${1:-default}"
来源：http://sxf.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://otw.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ycp.yj20258.top

[R07] if 判断文件
来源：http://kie.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cdt.bbcook.cn

[R08] 数值比较
来源：http://xpc.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ans.yfazqb.com

[R09] 字符串比较
来源：http://jve.c1oappe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qoe.0kj1m.cn

[R10] 正则匹配
来源：http://vin.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mru.zhengqikj.top

[R11] case 多分支
来源：http://ygr.jqgfzy.top

case "$1" in
来源：http://qql.hysaishi.cn

start) echo "启动" ;;
来源：http://cgi.yangfankeji.com

stop)  echo "停止" ;;
来源：http://veq.yonumen.top

*)     echo "未知命令" ;;
来源：http://yib.havefunace.top

esac
来源：http://pff.shzxlz.cn

[R12] for 遍历文件
来源：http://xmw.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://huk.316326.xyz

[R13] for 计数循环
来源：http://for.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://peh.yongpay.top

[R14] C 风格 for
来源：http://onk.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cud.jiagoushi.top

[R15] while 逐行读文件
来源：http://tvh.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tqh.yueranfly.top

[R16] until 等待条件
来源：http://aqk.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tpl.jqgufenzy.top

[R17] 数组定义与取值
来源：http://vhn.nanxinkj.top

arr=(a b c); echo "${arr[0]}"
来源：http://vpl.sufxvd.cn

[R18] 遍历数组
来源：http://eav.yj20258.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sfe.jianghu66.top

[R19] 数组长度
来源：http://xsf.yuxming.cn

echo "${#arr[@]}"
来源：http://eut.yongpay.top

[R20] 关联数组（字典）
来源：http://hts.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ofn.hnqzz.top

[R21] 字符串长度
来源：http://szw.ppjwa.cn

echo "${#s}"
来源：http://ugg.shuidangran.top

[R22] 截取子串
来源：http://buj.tanke756.top

echo "${s:0:5}"
来源：http://qwd.yuxming.cn

[R23] 字符串替换
来源：http://pue.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pzy.yj202588.top

[R24] 大小写转换
来源：http://cgk.cashguo.top

echo "${s^^}"; echo "${s,,}"
来源：http://flj.iojbl.cn

[R25] 去后缀 / 去前缀
来源：http://fek.ywan-chungtsiang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qlf.fktsv.cn

[R26] 命令替换
来源：http://uab.mhx1999.top

now=$(date +%F); echo "$now"
来源：http://ien.fktsv.cn

[R27] 算术展开
来源：http://jwg.sweek.top

echo $((1 + 2 * 3))
来源：http://zxw.smart0.xyz

[R28] 浮点运算
来源：http://grf.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://ucw.cucudq.cn

[R29] 定义函数
来源：http://xbf.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lks.jinqigufen.top

[R30] 函数返回状态码
来源：http://vvm.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://wtb.quarkkingdee.top

[R31] 局部变量
来源：http://teu.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://msj.fktsv.cn

[R32] 参数个数校验
来源：http://cxs.shanyushiyangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tes.52xcode.cn

[R33] 捕获错误并提示行号
来源：http://ega.gzhubu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nhb.feifeiyinyue.top

[R34] 退出时清理
来源：http://cwv.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://ygt.fanxiaobao.xyz

[R35] 后台执行并等待
来源：http://oaz.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nba.smart0.xyz

[R36] 并发执行多个任务
来源：http://gzy.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://htl.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://ahb.daxiang520.top

files=$(ls -1)
来源：http://drq.hysaishi.cn

[R38] 管道串联
来源：http://eaf.sysykeji.top

cat a.txt | grep -i error | wc -l
来源：http://ocu.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://ymb.iojbl.cn

cmd > out.log 2>&1
来源：http://mtw.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://khk.redwolf501.top

echo "log" >> out.log
来源：http://xlk.ppjwa.cn

[R41] 丢弃输出
来源：http://kus.yj20258.top

cmd >/dev/null 2>&1
来源：http://uoa.andypj.xyz

[R42] 输入重定向
来源：http://wyi.52xcode.cn

wc -l < a.txt
来源：http://tot.epnwcf.com

[R43] 按名字查找文件
来源：http://yjp.yangfankeji.com

find . -name "*.log" -type f
来源：http://kkw.yuxming.cn

[R44] 按修改时间查找
来源：http://ihu.xziqi.cn

find . -mtime -7 -type f
来源：http://rob.gaohongyu789.top

[R45] 批量删除
来源：http://pgo.birdmap.top

find . -name "*.tmp" -delete
来源：http://yyp.ppjwa.cn

[R46] 递归替换文件内容
来源：http://hgh.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gza.9152youxi.cn

[R47] sed 单行替换
来源：http://okp.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://maj.vqdsnc.cn

[R48] awk 取指定列
来源：http://nim.jinghuilouyu.cn

awk '{print $1, $3}' a.txt
来源：http://irt.vehdjk.com

[R49] awk 带条件
来源：http://gmn.9152youxi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lax.yj20258.top

[R50] awk 求和
来源：http://lnc.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mqy.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://fpi.52xcode.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://znl.ppjwa.cn

[R52] 统计行数
来源：http://ipo.uphjek.com

wc -l a.txt
来源：http://rez.uphjek.com

[R53] 查看文件头与实时尾
来源：http://xju.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://irw.shzxlz.cn

[R54] 比较两个文件
来源：http://eby.zhoulong.xyz

diff a.txt b.txt
来源：http://zef.guowangkeji.top

[R55] 压缩与解压
来源：http://zzy.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gzq.wangshuangyany.cn

[R56] 远程拷贝
来源：http://nfj.snrcjt.cn

scp file user@host:/path/
来源：http://jry.mhx1999.top

[R57] 远程执行命令
来源：http://kfj.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://jbt.sweek.top

[R58] 下载文件
来源：http://god.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://goa.yfazqb.com

[R59] 发 POST JSON
来源：http://knm.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ipm.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://ilv.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://exh.yfazqb.com

[R61] 磁盘占用
来源：http://pox.jinqigufen.top

df -h;  du -sh *
来源：http://ngc.fengsongda.top

[R62] 找最占空间的文件
来源：http://wgt.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://qtj.shanyushiyangtech.top

[R63] 内存与进程
来源：http://kge.yonumen.top

free -h;  ps aux | grep nginx
来源：http://anv.uphjek.com

[R64] 结束进程
来源：http://qwl.fanxiaobao.xyz

kill -9 $(pgrep -f app.py)
来源：http://uvi.hnxiangtu.top

[R65] 查看端口占用
来源：http://ndk.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yza.hnxiangtu.top

[R66] 定时任务
来源：http://mea.gzhubu.top

crontab -e;  crontab -l
来源：http://rdw.ivvv.top

[R67] 生成随机十六进制串
来源：http://byl.cqqwz.cn

openssl rand -hex 16
来源：http://tcm.zycfv.cn

[R68] 计算文件校验值
来源：http://mpl.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://joi.jinyuanbaomall.cn

[R69] 生成随机密码
来源：http://uqy.yj20258.top

head -c 16 /dev/urandom | base64
来源：http://vgh.daria6918.cn

[R70] 时间戳与互转
来源：http://rrz.yj20258888.top

date +%s;  date -d @1700000000
来源：http://tpn.jqgfzy.top

[R71] 日期格式化
来源：http://hwx.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qko.yj20258888.top

[R72] 等待端口就绪
来源：http://mfx.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://szp.hammf.cn

[R73] 分割大日志
来源：http://ecp.9152youxi.cn

split -l 1000 big.log part_
来源：http://ust.yuxming.cn

[R74] 批量重命名
来源：http://wii.dashuyun.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zuw.hfpthk.cn

[R75] 导出环境变量
来源：http://klf.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://abg.tian-w.cn

[R76] 使用临时文件
来源：http://fit.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rxo.cheryme.top

[R77] 读取用户输入
来源：http://gcc.hesvh.cn


<!-- 参考信息 -->