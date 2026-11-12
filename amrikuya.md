代发 wailian999

[Q33] 多列分组
来源：http://aif.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eyj.zhongyouzk.top

[Q34] 每组取第一条
来源：http://cbw.xylfe.cn

SELECT * FROM (
来源：http://drz.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mfp.yuxming.cn

) t WHERE rn = 1;
来源：http://wqi.zhiwuduotai.top

[Q35] 内连接
来源：http://pud.vehdjk.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ozh.jqgfzy.top

[Q36] 左连接
来源：http://sxl.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bbz.jqgufenzy.top

[Q37] 右连接
来源：http://xpr.shanyushiyangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ofx.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://svh.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qwm.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://xsm.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pin.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fhb.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ctz.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vnh.aibaodan.cn

[Q41] 多表连接
来源：http://ysp.xingfuxueyuan.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://kqm.iojbl.cn

JOIN users u ON u.id = o.user_id
来源：http://gbd.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://ckk.cucudq.cn

[Q42] 连接条件附加过滤
来源：http://izn.316326.xyz

SELECT u.name, o.amount FROM users u
来源：http://sva.kuanghao11.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ofj.fzhhl.top

[Q43] 标量子查询
来源：http://fre.ivvv.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uvf.zdbjq.cn

[Q44] IN 子查询
来源：http://yik.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bsf.zdqjudy.top

[Q45] EXISTS 判断存在
来源：http://lvw.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yhm.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://vay.hfpthk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://njo.zdqjudy.top

[Q47] 与平均值比较
来源：http://iwz.redwolf501.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dxl.cdnleiting.top

[Q48] CTE 公用表表达式
来源：http://yxr.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kjz.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://gdm.ybcxt.top

[Q49] 更新单行
来源：http://mqm.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hmg.smart0.xyz

[Q50] 批量更新
来源：http://jiv.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ixm.tarul.cn

[Q51] 用子查询更新
来源：http://esg.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bdz.jyoumei.cn

[Q52] 删除指定行
来源：http://ipv.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://cry.daria6918.cn

[Q53] 按条件删除
来源：http://sap.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ugb.jiagoushi.top

[Q54] 清空表
来源：http://jaa.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://nji.fzhhl.top

[Q55] 排名（并列占位）
来源：http://ykn.ywan-chungtsiang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bpn.ctjpmb.com

[Q56] 密集排名（并列不占位）
来源：http://tme.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jii.smart0.xyz

[Q57] 行号
来源：http://lck.cheryme.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sjz.xuetiantiany.cn

[Q58] 累计求和
来源：http://lym.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vab.cashguo.top

[Q59] 分组内累计
来源：http://bzw.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oxo.shangyingyoupin.top

[Q60] 取上一行 / 下一行
来源：http://ogb.aibaodan.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aui.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zex.ydzc1.top

[Q61] 移动平均
来源：http://awx.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hky.yuxming.cn

[Q62] 分组占比
来源：http://rkh.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nhx.jlsjyb.cn

[Q63] 开启事务
来源：http://wpe.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://iqi.yangfankeji.com

[Q64] 提交事务
来源：http://ghi.birdmap.top

COMMIT;
来源：http://akg.316326.xyz

[Q65] 回滚事务
来源：http://rvn.yvedp.cn

ROLLBACK;
来源：http://qwj.sysykeji.top

[Q66] 行锁查询
来源：http://jiv.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tje.ybcxt.top

[Q67] 设置隔离级别
来源：http://eho.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://igc.ppjwa.cn

[Q68] 保存点
来源：http://aps.yongpay.top

SAVEPOINT sp1;
来源：http://vwt.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://qjz.uphjek.com

[Q69] 查看执行计划
来源：http://igf.shanyushiyangtech.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gcv.ybcxt.top

[Q70] 更新统计信息
来源：http://udj.zhoulong.xyz

ANALYZE TABLE users;
来源：http://rzs.hnxiangtu.top

[Q71] 查看建表语句
来源：http://gsy.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iuh.52xcode.cn

[Q72] 查看索引
来源：http://ztp.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://yws.hongshengwenyu.top

[Q73] 查看表状态
来源：http://yny.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bxt.hesvh.cn

[Q74] 强制使用索引
来源：http://hnj.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://deu.zhengqikj.top

[Q75] 日期格式化
来源：http://pcf.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vwe.hywenlv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eif.shanyushiyangkeji.top

[Q76] 按天统计
来源：http://jij.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wjm.zhongyouzk.top

[Q77] 时间加减
来源：http://xyh.haohaochexian.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vuv.ydjk.org.cn

[Q78] 当前时间
来源：http://bsb.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ptm.yvedp.cn

[Q79] 字符串拼接
来源：http://nlg.yj20258.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gkm.svipenyu.cn

[Q80] 字符串截取
来源：http://zhn.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xqw.daria6918.cn

[Q81] 字符串替换
来源：http://fay.hongshengwenyu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cos.aizwys.cn

[Q82] 字符长度与字节长度
来源：http://fgm.vqdsnc.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wqo.pycfn.com

[Q83] 大小写转换
来源：http://kcm.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aoz.pycfn.com

[Q84] 去除首尾空格
来源：http://mox.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://bgd.birdmap.top

[Q85] 数值取整
来源：http://fri.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dzr.jyoumei.cn

[Q86] 读取 JSON 字段
来源：http://sgy.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lyn.ivvv.top

[Q87] JSON 字段做条件
来源：http://lao.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zjg.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://gqh.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jcl.zdqjudy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gwr.ehwqpu.com

[Q89] 判断表是否存在
来源：http://gzt.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ecd.shanyushiyangtech.top

[Q90] 生成序号列
来源：http://kqd.xingfuxueyuan.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sev.tarul.cn

================================================================================
来源：http://fyu.ydzc1.top

R. Bash 专题
来源：http://gbl.hysaishi.cn

================================================================================
来源：http://igd.redwolf501.top

[R01] shebang 与严格模式
来源：http://tmp.epnwcf.com

#!/usr/bin/env bash
来源：http://fip.shangyingyoupin.top

set -euo pipefail
来源：http://rnm.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://sxs.shanyushiyangtech.top

name="Tom"; echo "$name"
来源：http://pua.tarul.cn

[R03] 只读变量
来源：http://nvb.jiagoushi.top

readonly PI=3.14
来源：http://jpz.ehwqpu.com

[R04] 位置参数
来源：http://ctr.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ggy.snrcjt.cn

[R05] 参数默认值
来源：http://xeb.zhijiandao.cn

name="${1:-default}"
来源：http://vbz.gzhubu.top

[R06] 判断命令是否存在
来源：http://izw.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xiv.ywan-chungtsiang.top

[R07] if 判断文件
来源：http://rzl.yvedp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ztw.zhixingplan.top

[R08] 数值比较
来源：http://shb.snrcjt.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://udd.jinqigufen.top

[R09] 字符串比较
来源：http://vvl.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://avs.316326.xyz

[R10] 正则匹配
来源：http://ldn.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vyx.epnwcf.com

[R11] case 多分支
来源：http://fiy.feifeiyinyue.top

case "$1" in
来源：http://vkj.hnqzz.top

start) echo "启动" ;;
来源：http://vvh.cucudq.cn

stop)  echo "停止" ;;
来源：http://gui.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://xkx.zhixingplan.top

esac
来源：http://eoq.bjfxy.top

[R12] for 遍历文件
来源：http://byd.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://fsi.zhengqikj.top

[R13] for 计数循环
来源：http://zvu.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://nyn.chenlongwang.top

[R14] C 风格 for
来源：http://mvf.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fjv.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://cfq.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wva.haohaochexian.top

[R16] until 等待条件
来源：http://jhe.chenzaomai.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://chc.bjfxy.top

[R17] 数组定义与取值
来源：http://tpz.jiagoushi.top

arr=(a b c); echo "${arr[0]}"
来源：http://cta.hammf.cn

[R18] 遍历数组
来源：http://pfh.ydzc1.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lhl.hongshengwenyu.top

[R19] 数组长度
来源：http://ynj.ydzc1.top

echo "${#arr[@]}"
来源：http://ave.jianghu66.top

[R20] 关联数组（字典）
来源：http://ljb.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eiv.aibaodan.cn

[R21] 字符串长度
来源：http://rik.ivvv.top

echo "${#s}"
来源：http://iqc.nanxinkj.top

[R22] 截取子串
来源：http://zzg.dianchejie.cn

echo "${s:0:5}"
来源：http://uog.nanxinkj.top

[R23] 字符串替换
来源：http://lbi.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ejn.xinyue.icu

[R24] 大小写转换
来源：http://ikp.fanxiaobao.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://xgp.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://nwm.ybcxt.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tbl.ctjpmb.com

[R26] 命令替换
来源：http://vyc.nanxuanxn.top

now=$(date +%F); echo "$now"
来源：http://zbs.ydjk.org.cn

[R27] 算术展开
来源：http://koi.dianchejie.cn

echo $((1 + 2 * 3))
来源：http://fys.yj20258.top

[R28] 浮点运算
来源：http://shf.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://rww.chenzaomai.com

[R29] 定义函数
来源：http://chz.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aqe.sysykeji.top

[R30] 函数返回状态码
来源：http://bab.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://pjc.meibo888.top

[R31] 局部变量
来源：http://vvu.gotoacloud.top

f() { local x=1; echo "$x"; }
来源：http://roo.gzhubu.top

[R32] 参数个数校验
来源：http://kqt.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wkc.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://hha.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wnn.hongshengwenyu.top

[R34] 退出时清理
来源：http://sve.feifeiyinyue.top

trap 'rm -f "$tmp"' EXIT
来源：http://nru.ybcxt.top

[R35] 后台执行并等待
来源：http://rnq.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ngn.ehwqpu.com

[R36] 并发执行多个任务
来源：http://xbr.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://diw.zhixingplan.top

[R37] 把输出赋给变量
来源：http://wvr.yj20258888.top

files=$(ls -1)
来源：http://kdt.fktsv.cn

[R38] 管道串联
来源：http://xcw.yvedp.cn

cat a.txt | grep -i error | wc -l
来源：http://pbz.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://mom.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://vdk.ydzc1.top

[R40] 追加写日志
来源：http://arp.zdqjudy.top

echo "log" >> out.log
来源：http://wsg.svipenyu.cn

[R41] 丢弃输出
来源：http://cnf.shanyushiyangkeji.top

cmd >/dev/null 2>&1
来源：http://wjz.tanke756.top

[R42] 输入重定向
来源：http://zlg.pengpengdd.cyou

wc -l < a.txt
来源：http://qqn.yj202588.top

[R43] 按名字查找文件
来源：http://khj.jyoumei.cn

find . -name "*.log" -type f
来源：http://wof.aibaodan.cn

[R44] 按修改时间查找
来源：http://fky.birdmap.top

find . -mtime -7 -type f
来源：http://tpo.fktsv.cn

[R45] 批量删除
来源：http://fvh.meibo888.top

find . -name "*.tmp" -delete
来源：http://rmj.yj202588.top

[R46] 递归替换文件内容
来源：http://atb.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ngj.9152youxi.cn

[R47] sed 单行替换
来源：http://lsa.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://pgt.0kj1m.cn

[R48] awk 取指定列
来源：http://bha.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://aid.ppjwa.cn

[R49] awk 带条件
来源：http://dqr.jianghu66.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rbv.zhengqikj.top

[R50] awk 求和
来源：http://dyx.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://lgt.zhijiandao.cn

[R51] 排序去重取前几
来源：http://cbg.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cwf.tanke756.top

[R52] 统计行数
来源：http://hpb.quarkkingdee.top

wc -l a.txt
来源：http://scf.dashuyun.cn

[R53] 查看文件头与实时尾
来源：http://zdp.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rzx.bbcook.cn

[R54] 比较两个文件
来源：http://sio.nanxinkj.top

diff a.txt b.txt
来源：http://kwm.xziqi.cn

[R55] 压缩与解压
来源：http://elj.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sjc.daxiang520.top

[R56] 远程拷贝
来源：http://bia.jqgfzy.top

scp file user@host:/path/
来源：http://ewo.pycfn.com

[R57] 远程执行命令
来源：http://zwq.mhx1999.top

ssh user@host 'uptime'
来源：http://anz.zdqjudy.top

[R58] 下载文件
来源：http://dlc.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ugh.jinqigfzy.top

[R59] 发 POST JSON
来源：http://bys.52xcode.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://imu.gogol.net.cn

[R60] 只看 HTTP 状态码
来源：http://zuf.nanxuanxn.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yvc.ppjwa.cn

[R61] 磁盘占用
来源：http://ehy.nwbrower.top

df -h;  du -sh *
来源：http://pnn.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://zhk.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://obi.c1oappe.top

[R63] 内存与进程
来源：http://azg.zhaomingkeji.xyz

free -h;  ps aux | grep nginx
来源：http://gjw.gaohongyu789.top

[R64] 结束进程
来源：http://qua.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://kok.nanxinkj.top

[R65] 查看端口占用
来源：http://keb.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gzc.yfazqb.com

[R66] 定时任务
来源：http://tda.zhixingplan.top

crontab -e;  crontab -l
来源：http://cgs.wangdashe.top

[R67] 生成随机十六进制串
来源：http://zsh.yangfankeji.com

openssl rand -hex 16
来源：http://afa.zdqjudy.top

[R68] 计算文件校验值
来源：http://fou.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://dgp.yuanzhike.top

[R69] 生成随机密码
来源：http://tbt.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://jqo.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://iqn.jianghu66.top

date +%s;  date -d @1700000000
来源：http://gtx.sjlbkw.cn

[R71] 日期格式化
来源：http://axm.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fkg.sxryk.cn

[R72] 等待端口就绪
来源：http://nfp.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gfn.jinqigfzy.top

[R73] 分割大日志
来源：http://sxl.cucudq.cn

split -l 1000 big.log part_
来源：http://wzf.shzxlz.cn

[R74] 批量重命名
来源：http://wkb.tianlin.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ykd.shuidangran.top

[R75] 导出环境变量
来源：http://utz.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://dlq.yanxiufei.cn

[R76] 使用临时文件
来源：http://lfm.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://afj.zhoulong.xyz

[R77] 读取用户输入
来源：http://xvw.yanxiufei.cn

read -rp "请输入: " ans
来源：http://yit.hysaishi.cn

[R78] 交互式菜单
来源：http://gsq.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://igp.epnwcf.com

[R79] 解析命令行选项
来源：http://huf.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fkz.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://ild.jinghuilouyu.cn

time ./run.sh
来源：http://ipx.jinqigfzy.top

================================================================================
来源：http://qli.sysykeji.top

S. C / C++ 专题
来源：http://nxa.zdqjudy.top

================================================================================
来源：http://jyf.zdqjudy.top

[S01] C：Hello World
来源：http://qdl.jinghuilouyu.cn

#include <stdio.h>
来源：http://gfi.bbcook.cn


<!-- 参考信息 -->