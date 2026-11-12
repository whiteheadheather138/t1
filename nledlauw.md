代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nlf.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://ric.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tcb.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vgf.quarkkingdee.top

[Q33] 多列分组
来源：http://vyj.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rmx.cashguo.top

[Q34] 每组取第一条
来源：http://akp.dashuyun.cn

SELECT * FROM (
来源：http://zyo.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xka.fengsongda.top

) t WHERE rn = 1;
来源：http://uvc.tian-w.cn

[Q35] 内连接
来源：http://the.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kon.iojbl.cn

[Q36] 左连接
来源：http://bmo.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rdr.smart0.xyz

[Q37] 右连接
来源：http://jdg.andypj.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uzz.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://bpa.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nkk.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://ivh.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wht.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hru.chenjidiqi.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://nqu.jinghuilouyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rfq.zhijiandao.cn

[Q41] 多表连接
来源：http://nna.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mgf.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://rqz.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://agl.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://kly.pycfn.com

SELECT u.name, o.amount FROM users u
来源：http://qkn.hfpthk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fuz.gzhubu.top

[Q43] 标量子查询
来源：http://tsx.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://phb.hysaishi.cn

[Q44] IN 子查询
来源：http://mhz.ivvv.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bab.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://csa.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rkh.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://szx.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jfb.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://ttk.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ryr.daxiang520.top

[Q48] CTE 公用表表达式
来源：http://jsk.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dox.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ytr.fktsv.cn

[Q49] 更新单行
来源：http://kjf.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wpz.xuanzx.com

[Q50] 批量更新
来源：http://sqg.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jul.epnwcf.com

[Q51] 用子查询更新
来源：http://zxn.yueranfly.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vdb.xziqi.cn

[Q52] 删除指定行
来源：http://bnv.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://hhq.fanxiaobao.xyz

[Q53] 按条件删除
来源：http://yla.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cqt.tanke756.top

[Q54] 清空表
来源：http://uvl.bjfxy.top

TRUNCATE TABLE logs;
来源：http://cez.yvedp.cn

[Q55] 排名（并列占位）
来源：http://jcu.jqgfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eum.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://fgu.hnqzz.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://atp.zhijiandao.cn

[Q57] 行号
来源：http://ulg.hongshengwenyu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yfr.ctjpmb.com

[Q58] 累计求和
来源：http://uzw.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pvg.xuetiantiany.cn

[Q59] 分组内累计
来源：http://bug.jinqigufen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xsu.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://erm.jlsjyb.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gwy.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://drm.gaohongyu789.top

[Q61] 移动平均
来源：http://lxm.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nze.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://ype.tian-w.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pfk.aizwys.cn

[Q63] 开启事务
来源：http://cex.pycfn.com

START TRANSACTION;                -- 或 BEGIN
来源：http://bpb.bjfxy.top

[Q64] 提交事务
来源：http://jhq.kuanghao11.cn

COMMIT;
来源：http://act.dashuyun.cn

[Q65] 回滚事务
来源：http://oni.c1oappe.top

ROLLBACK;
来源：http://ucc.tian-w.cn

[Q66] 行锁查询
来源：http://zbk.9152youxi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qtp.uphjek.com

[Q67] 设置隔离级别
来源：http://uqi.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ylk.ydzc1.top

[Q68] 保存点
来源：http://oyl.yongpay.top

SAVEPOINT sp1;
来源：http://plp.yuanzhike.top

ROLLBACK TO sp1;
来源：http://lxl.cucudq.cn

[Q69] 查看执行计划
来源：http://ljs.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ckv.cucudq.cn

[Q70] 更新统计信息
来源：http://tph.uphjek.com

ANALYZE TABLE users;
来源：http://snq.nwbrower.top

[Q71] 查看建表语句
来源：http://gvd.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://net.9152youxi.cn

[Q72] 查看索引
来源：http://vho.jqgfzy.top

SHOW INDEX FROM users;
来源：http://hfx.gotoacloud.top

[Q73] 查看表状态
来源：http://hta.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://syd.jianghu66.top

[Q74] 强制使用索引
来源：http://iki.jinqigufen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kqr.gaohongyu789.top

[Q75] 日期格式化
来源：http://yvk.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xcz.daxiang520.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oyy.guannengcc.top

[Q76] 按天统计
来源：http://qxf.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mml.wangdashe.top

[Q77] 时间加减
来源：http://uey.gaohongyu789.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iez.havefunace.top

[Q78] 当前时间
来源：http://fcl.zhiwuduotai.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hov.cheryme.top

[Q79] 字符串拼接
来源：http://isw.zycfv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qmy.jinqigufen.top

[Q80] 字符串截取
来源：http://sgu.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://irh.hnqzz.top

[Q81] 字符串替换
来源：http://qao.xingfuxueyuan.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xzf.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://vhr.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nxn.yj20258.top

[Q83] 大小写转换
来源：http://rde.nanxuanxn.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jef.yj20258.top

[Q84] 去除首尾空格
来源：http://qlg.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://ala.tian-w.cn

[Q85] 数值取整
来源：http://htx.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dnj.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://zdt.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lvl.sweek.top

[Q87] JSON 字段做条件
来源：http://qpg.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jza.ydjk.org.cn

[Q88] 行转列（条件聚合）
来源：http://tst.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tbg.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xff.dashuyun.cn

[Q89] 判断表是否存在
来源：http://mhp.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://txr.yj20258.top

[Q90] 生成序号列
来源：http://mwx.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://exp.sysykeji.top

================================================================================
来源：http://hni.mhx1999.top

R. Bash 专题
来源：http://enz.316326.xyz

================================================================================
来源：http://ldj.zhixingplan.top

[R01] shebang 与严格模式
来源：http://gxz.wangdashe.top

#!/usr/bin/env bash
来源：http://zyo.ybcxt.top

set -euo pipefail
来源：http://vai.nwbrower.top

[R02] 变量赋值与使用
来源：http://llg.daxiang520.top

name="Tom"; echo "$name"
来源：http://zaf.xuanzx.com

[R03] 只读变量
来源：http://szi.yangfankeji.com

readonly PI=3.14
来源：http://yyc.fktsv.cn

[R04] 位置参数
来源：http://nqe.fengsongda.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wth.sweek.top

[R05] 参数默认值
来源：http://dmz.hesvh.cn

name="${1:-default}"
来源：http://zqo.hongshengwenyu.top

[R06] 判断命令是否存在
来源：http://rni.0kj1m.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xqs.nanxinkj.top

[R07] if 判断文件
来源：http://usk.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wrg.cheryme.top

[R08] 数值比较
来源：http://wxh.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://kvc.uphjek.com

[R09] 字符串比较
来源：http://tdc.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vus.hcnkem.com

[R10] 正则匹配
来源：http://ymr.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ikp.bbcook.cn

[R11] case 多分支
来源：http://svd.fehbvm.com

case "$1" in
来源：http://yci.cdnleiting.top

start) echo "启动" ;;
来源：http://jza.yvedp.cn

stop)  echo "停止" ;;
来源：http://nqx.xuetiantiany.cn

*)     echo "未知命令" ;;
来源：http://mgu.xingfuxueyuan.xyz

esac
来源：http://hor.zhiwuduotai.top

[R12] for 遍历文件
来源：http://diu.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://cvi.yj202588.top

[R13] for 计数循环
来源：http://ehz.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://ufa.yuanzhike.top

[R14] C 风格 for
来源：http://lfv.jinyuanbaomall.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cox.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://ifb.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xvs.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://byw.yuanzhike.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wlw.yj202588.top

[R17] 数组定义与取值
来源：http://gck.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yjx.9152youxi.cn

[R18] 遍历数组
来源：http://ybf.fktsv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fqq.iojbl.cn

[R19] 数组长度
来源：http://bvk.havefunace.top

echo "${#arr[@]}"
来源：http://udn.52xcode.cn

[R20] 关联数组（字典）
来源：http://eke.zhixingplan.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tab.gaohongyu789.top

[R21] 字符串长度
来源：http://xjc.yvedp.cn

echo "${#s}"
来源：http://bml.cdnleiting.top

[R22] 截取子串
来源：http://ifs.xylfe.cn

echo "${s:0:5}"
来源：http://pqm.jinqigfzy.top

[R23] 字符串替换
来源：http://swu.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rjd.zhixingplan.top

[R24] 大小写转换
来源：http://rjs.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fdr.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://blf.zhengqikj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lag.hysaishi.cn

[R26] 命令替换
来源：http://mxz.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://hro.nwbrower.top

[R27] 算术展开
来源：http://kta.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://pxx.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://nmb.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://juy.svipenyu.cn

[R29] 定义函数
来源：http://iwg.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qjw.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://cqg.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://nhb.tarul.cn

[R31] 局部变量
来源：http://rgr.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://ibd.hfpthk.cn

[R32] 参数个数校验
来源：http://svj.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rbu.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://hiy.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jna.yvedp.cn

[R34] 退出时清理
来源：http://yao.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vub.yonumen.top

[R35] 后台执行并等待
来源：http://nof.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bew.wangshuangyany.cn

[R36] 并发执行多个任务
来源：http://qrs.nanxuanxn.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qax.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://crz.ppjwa.cn

files=$(ls -1)
来源：http://ofk.jqgufenzy.top

[R38] 管道串联
来源：http://hra.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://yts.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://vca.cashguo.top

cmd > out.log 2>&1
来源：http://ywx.ivvv.top

[R40] 追加写日志
来源：http://zox.hnqzz.top

echo "log" >> out.log
来源：http://phu.yangfankeji.com

[R41] 丢弃输出
来源：http://mqd.aibaodan.cn

cmd >/dev/null 2>&1
来源：http://zvq.zycfv.cn

[R42] 输入重定向
来源：http://jdt.quarkkingdee.top

wc -l < a.txt
来源：http://ftr.chenzaomai.com

[R43] 按名字查找文件
来源：http://ndf.316326.xyz

find . -name "*.log" -type f
来源：http://fqd.shzxlz.cn

[R44] 按修改时间查找
来源：http://xnp.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://pce.sjlbkw.cn

[R45] 批量删除
来源：http://dfw.zhongyouzk.top

find . -name "*.tmp" -delete
来源：http://uqc.52xcode.cn

[R46] 递归替换文件内容
来源：http://ega.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://isk.aizwys.cn

[R47] sed 单行替换
来源：http://hyb.zhiwuduotai.top

sed -i 's/foo/bar/g' a.txt
来源：http://mtx.xylfe.cn

[R48] awk 取指定列
来源：http://ycq.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://aop.hcnkem.com

[R49] awk 带条件
来源：http://kmx.uphjek.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cmm.guowangkeji.top

[R50] awk 求和
来源：http://bqt.wangdashe.top

awk '{s += $2} END {print s}' a.txt
来源：http://ode.cdnleiting.top

[R51] 排序去重取前几
来源：http://xhu.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kxy.yangfankeji.com

[R52] 统计行数
来源：http://yju.gzhubu.top

wc -l a.txt
来源：http://cvi.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://cbn.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iqs.jinyuanbaomall.cn

[R54] 比较两个文件
来源：http://vwx.xuanzx.com

diff a.txt b.txt
来源：http://nmn.sysykeji.top

[R55] 压缩与解压
来源：http://sis.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nao.yanxiufei.cn

[R56] 远程拷贝
来源：http://ogf.fanxiaobao.xyz

scp file user@host:/path/
来源：http://xgp.cashguo.top

[R57] 远程执行命令
来源：http://ogq.zhixingplan.top

ssh user@host 'uptime'
来源：http://doo.nwbrower.top

[R58] 下载文件
来源：http://ezr.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wun.cdnleiting.top

[R59] 发 POST JSON
来源：http://rkk.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zwe.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://gcd.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://amg.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://jop.c1oappe.top

df -h;  du -sh *
来源：http://bif.yj20258.top

[R62] 找最占空间的文件
来源：http://qpj.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://anh.ydjk.org.cn

[R63] 内存与进程
来源：http://fhe.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://som.uphjek.com

[R64] 结束进程
来源：http://smr.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://zoh.wangdashe.top

[R65] 查看端口占用
来源：http://dst.shanyushiyangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://teb.ctjpmb.com

[R66] 定时任务
来源：http://ukg.hywenlv.cn

crontab -e;  crontab -l
来源：http://gqh.zhoulong.xyz

[R67] 生成随机十六进制串
来源：http://twa.zhiwuduotai.top

openssl rand -hex 16
来源：http://hai.hywenlv.cn

[R68] 计算文件校验值
来源：http://vzg.ydzc1.top

sha256sum a.txt;  md5sum a.txt
来源：http://dly.quarkkingdee.top

[R69] 生成随机密码
来源：http://vgu.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://fod.xinyue.icu

[R70] 时间戳与互转
来源：http://rti.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://blb.sweek.top

[R71] 日期格式化
来源：http://jja.zhengqikj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rar.yuxming.cn

[R72] 等待端口就绪
来源：http://rco.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://juj.jyoumei.cn

[R73] 分割大日志
来源：http://fez.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://vpf.zhijiandao.cn

[R74] 批量重命名
来源：http://foa.52xcode.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xtb.yanxiufei.cn

[R75] 导出环境变量
来源：http://jqu.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://qad.tanke756.top

[R76] 使用临时文件
来源：http://dzh.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ovu.jinqigufen.top

[R77] 读取用户输入
来源：http://ezt.havefunace.top

read -rp "请输入: " ans
来源：http://gyh.sysykeji.top

[R78] 交互式菜单
来源：http://zbg.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wvw.bbcook.cn

[R79] 解析命令行选项
来源：http://dbc.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ixt.yonumen.top

[R80] 查看脚本执行耗时
来源：http://qyx.andypj.xyz

time ./run.sh
来源：http://rxj.cucudq.cn

================================================================================
来源：http://hph.yonumen.top


<!-- 参考信息 -->