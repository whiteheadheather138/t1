代发 wailian999

[Q36] 左连接
来源：http://lnf.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sor.jinghuilouyu.cn

[Q37] 右连接
来源：http://irr.jinqigfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pfd.0kj1m.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mwp.haohaochexian.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ike.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://hop.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://rbo.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sly.hfpthk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fnc.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vol.dianchejie.cn

[Q41] 多表连接
来源：http://ldv.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://apy.xingfuxueyuan.xyz

JOIN users u ON u.id = o.user_id
来源：http://mas.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://yhp.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://wsa.mhx1999.top

SELECT u.name, o.amount FROM users u
来源：http://bzj.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://alt.ehwqpu.com

[Q43] 标量子查询
来源：http://fsx.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rhf.yueranfly.top

[Q44] IN 子查询
来源：http://bql.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cnl.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://bjl.zdqjudy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://btk.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://pbr.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mcg.fzhhl.top

[Q47] 与平均值比较
来源：http://kns.sxryk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://miz.c1oappe.top

[Q48] CTE 公用表表达式
来源：http://kgn.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mjx.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://cff.bbcook.cn

[Q49] 更新单行
来源：http://ndc.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://woy.xylfe.cn

[Q50] 批量更新
来源：http://cjy.quarkkingdee.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rnu.yuanzhike.top

[Q51] 用子查询更新
来源：http://dyv.nanxuanxn.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gfm.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://dsx.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://fna.jinyuanbaomall.cn

[Q53] 按条件删除
来源：http://wmi.tanke756.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xxs.sweek.top

[Q54] 清空表
来源：http://iyk.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://wsu.smart0.xyz

[Q55] 排名（并列占位）
来源：http://aye.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cox.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://ysm.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hld.smart0.xyz

[Q57] 行号
来源：http://zgw.52xcode.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ktv.ctjpmb.com

[Q58] 累计求和
来源：http://nts.zhengqikj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jxm.shanyushiyangtech.top

[Q59] 分组内累计
来源：http://bcl.sufxvd.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oiu.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://kln.tianlin.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://exv.sufxvd.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wfi.hnxiangtu.top

[Q61] 移动平均
来源：http://cwx.wangshuangyany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yej.hnxiangtu.top

[Q62] 分组占比
来源：http://mvs.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hzy.pengpengdd.cyou

[Q63] 开启事务
来源：http://nzu.nanxinkj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jwe.hnxiangtu.top

[Q64] 提交事务
来源：http://eus.pycfn.com

COMMIT;
来源：http://vya.tarul.cn

[Q65] 回滚事务
来源：http://yga.hywenlv.cn

ROLLBACK;
来源：http://hhr.yanxiufei.cn

[Q66] 行锁查询
来源：http://lkg.zhongyouzk.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tof.uphjek.com

[Q67] 设置隔离级别
来源：http://qiy.sjlbkw.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hvw.aizwys.cn

[Q68] 保存点
来源：http://fjg.bjfxy.top

SAVEPOINT sp1;
来源：http://mnw.wangshuangyany.cn

ROLLBACK TO sp1;
来源：http://ghj.andypj.xyz

[Q69] 查看执行计划
来源：http://zrz.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pai.feifeiyinyue.top

[Q70] 更新统计信息
来源：http://vjd.hnxiangtu.top

ANALYZE TABLE users;
来源：http://clk.yongpay.top

[Q71] 查看建表语句
来源：http://khn.316326.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tyq.yj20258888.top

[Q72] 查看索引
来源：http://jsc.aibaodan.cn

SHOW INDEX FROM users;
来源：http://kbj.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://kpc.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://xco.chenzaomai.com

[Q74] 强制使用索引
来源：http://krq.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hgu.epnwcf.com

[Q75] 日期格式化
来源：http://jye.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zua.hammf.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kmn.yuxming.cn

[Q76] 按天统计
来源：http://rhy.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kbt.bjfxy.top

[Q77] 时间加减
来源：http://znw.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dvq.yuxming.cn

[Q78] 当前时间
来源：http://zhe.zhengqikj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gxj.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://lzt.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aty.zdbjq.cn

[Q80] 字符串截取
来源：http://ttg.yonumen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ggx.xinyue.icu

[Q81] 字符串替换
来源：http://eoa.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://miw.xingfuxueyuan.xyz

[Q82] 字符长度与字节长度
来源：http://mhn.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wxp.0kj1m.cn

[Q83] 大小写转换
来源：http://dun.xuanzx.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vda.52xcode.cn

[Q84] 去除首尾空格
来源：http://epa.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://hiv.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://lst.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fzu.shanyushiyangtech.top

[Q86] 读取 JSON 字段
来源：http://akk.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dee.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://qyo.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dfz.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://gve.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yvq.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://emn.cqqwz.cn

[Q89] 判断表是否存在
来源：http://dcu.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zca.jinqigufen.top

[Q90] 生成序号列
来源：http://jce.c1oappe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ehg.hfpthk.cn

================================================================================
来源：http://voh.zhixingplan.top

R. Bash 专题
来源：http://mht.sjlbkw.cn

================================================================================
来源：http://zzd.9152youxi.cn

[R01] shebang 与严格模式
来源：http://ghq.jyoumei.cn

#!/usr/bin/env bash
来源：http://zcg.ydzc1.top

set -euo pipefail
来源：http://smp.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://pay.cucudq.cn

name="Tom"; echo "$name"
来源：http://kxp.mhx1999.top

[R03] 只读变量
来源：http://zge.quarkkingdee.top

readonly PI=3.14
来源：http://kwd.gzhubu.top

[R04] 位置参数
来源：http://yho.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zne.yongpay.top

[R05] 参数默认值
来源：http://dea.ywan-chungtsiang.top

name="${1:-default}"
来源：http://diz.birdmap.top

[R06] 判断命令是否存在
来源：http://ure.iojbl.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vru.nwbrower.top

[R07] if 判断文件
来源：http://yjz.9152youxi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fwe.tianlin.xyz

[R08] 数值比较
来源：http://gxu.iojbl.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mts.yfazqb.com

[R09] 字符串比较
来源：http://xul.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ivf.nwbrower.top

[R10] 正则匹配
来源：http://tqi.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zfd.ywan-chungtsiang.top

[R11] case 多分支
来源：http://fjp.chenjidiqi.icu

case "$1" in
来源：http://ykj.jyoumei.cn

start) echo "启动" ;;
来源：http://cvm.dianchejie.cn

stop)  echo "停止" ;;
来源：http://drk.smart0.xyz

*)     echo "未知命令" ;;
来源：http://oly.vqdsnc.cn

esac
来源：http://hkc.ppjwa.cn

[R12] for 遍历文件
来源：http://sxd.c1oappe.top

for f in *.txt; do echo "$f"; done
来源：http://tbp.hysaishi.cn

[R13] for 计数循环
来源：http://czr.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://mst.hongshengwenyu.top

[R14] C 风格 for
来源：http://dov.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://erl.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://rdg.shanyushiyangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mvc.uphjek.com

[R16] until 等待条件
来源：http://kjd.iojbl.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://efk.sysykeji.top

[R17] 数组定义与取值
来源：http://kle.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://aed.nanxuanxn.top

[R18] 遍历数组
来源：http://uao.hysaishi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vbe.tanke756.top

[R19] 数组长度
来源：http://kzx.jianghu66.top

echo "${#arr[@]}"
来源：http://cjy.tian-w.cn

[R20] 关联数组（字典）
来源：http://czy.c1oappe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dvg.shangyingyoupin.top

[R21] 字符串长度
来源：http://mqp.shanyushiyangtech.top

echo "${#s}"
来源：http://zic.yvedp.cn

[R22] 截取子串
来源：http://nmi.tarul.cn

echo "${s:0:5}"
来源：http://zna.bbcook.cn

[R23] 字符串替换
来源：http://rwp.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ebp.zhixingplan.top

[R24] 大小写转换
来源：http://opb.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://kgl.iojbl.cn

[R25] 去后缀 / 去前缀
来源：http://mfq.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rvu.yonumen.top

[R26] 命令替换
来源：http://mcu.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://wts.mhx1999.top

[R27] 算术展开
来源：http://wov.cheryme.top

echo $((1 + 2 * 3))
来源：http://ojl.cdnleiting.top

[R28] 浮点运算
来源：http://yrp.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://izi.tarul.cn

[R29] 定义函数
来源：http://wlo.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kdx.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://djk.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://ejq.hammf.cn

[R31] 局部变量
来源：http://lto.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://eca.fanxiaobao.xyz

[R32] 参数个数校验
来源：http://hru.xinyue.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jiq.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://gdw.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wwd.yangfankeji.com

[R34] 退出时清理
来源：http://nct.yj20258.top

trap 'rm -f "$tmp"' EXIT
来源：http://kck.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://lft.ybcxt.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fck.cucudq.cn

[R36] 并发执行多个任务
来源：http://sxx.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zqb.daxiang520.top

[R37] 把输出赋给变量
来源：http://pwf.fehbvm.com

files=$(ls -1)
来源：http://pnf.hcnkem.com

[R38] 管道串联
来源：http://izi.nwbrower.top

cat a.txt | grep -i error | wc -l
来源：http://hbf.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://jrq.hesvh.cn

cmd > out.log 2>&1
来源：http://sou.redwolf501.top

[R40] 追加写日志
来源：http://uuu.shangyingyoupin.top

echo "log" >> out.log
来源：http://skf.zhoulong.xyz

[R41] 丢弃输出
来源：http://dfr.yuxming.cn

cmd >/dev/null 2>&1
来源：http://ibt.dianchejie.cn

[R42] 输入重定向
来源：http://iuz.ydzc1.top

wc -l < a.txt
来源：http://yyi.ivvv.top

[R43] 按名字查找文件
来源：http://pob.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://ihx.havefunace.top

[R44] 按修改时间查找
来源：http://uln.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://qiy.zycfv.cn

[R45] 批量删除
来源：http://jmr.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://ayt.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://veu.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kky.kuanghao11.cn

[R47] sed 单行替换
来源：http://dmt.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://zsy.hammf.cn

[R48] awk 取指定列
来源：http://hth.ydjk.org.cn

awk '{print $1, $3}' a.txt
来源：http://nly.hnqzz.top

[R49] awk 带条件
来源：http://xxx.fanxiaobao.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mqy.daxiang520.top

[R50] awk 求和
来源：http://zot.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vkz.cucudq.cn

[R51] 排序去重取前几
来源：http://dhv.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://koc.ppjwa.cn

[R52] 统计行数
来源：http://qgv.yanxiufei.cn

wc -l a.txt
来源：http://jlg.316326.xyz

[R53] 查看文件头与实时尾
来源：http://jhm.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://guy.yuxming.cn

[R54] 比较两个文件
来源：http://hjx.c1oappe.top

diff a.txt b.txt
来源：http://hbq.vehdjk.com

[R55] 压缩与解压
来源：http://zlx.yongpay.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://efm.havefunace.top

[R56] 远程拷贝
来源：http://qep.sysykeji.top

scp file user@host:/path/
来源：http://znq.quarkkingdee.top

[R57] 远程执行命令
来源：http://xrd.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://upn.yueranfly.top

[R58] 下载文件
来源：http://hog.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qxy.cucudq.cn

[R59] 发 POST JSON
来源：http://tgw.sweek.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cwn.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://mnk.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://puo.havefunace.top

[R61] 磁盘占用
来源：http://zkb.xziqi.cn

df -h;  du -sh *
来源：http://lyy.jqgufenzy.top

[R62] 找最占空间的文件
来源：http://mih.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://nwn.9152youxi.cn

[R63] 内存与进程
来源：http://rsk.tian-w.cn

free -h;  ps aux | grep nginx
来源：http://gjo.jiagoushi.top

[R64] 结束进程
来源：http://uqa.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://tei.yfazqb.com

[R65] 查看端口占用
来源：http://wrm.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lzl.tianlin.xyz

[R66] 定时任务
来源：http://xxt.hnxiangtu.top

crontab -e;  crontab -l
来源：http://kmk.gogol.net.cn

[R67] 生成随机十六进制串
来源：http://vwl.zycfv.cn

openssl rand -hex 16
来源：http://fjc.snrcjt.cn

[R68] 计算文件校验值
来源：http://msj.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://hqm.gzhubu.top

[R69] 生成随机密码
来源：http://nkf.hnqzz.top

head -c 16 /dev/urandom | base64
来源：http://qcj.jinqigufen.top

[R70] 时间戳与互转
来源：http://eau.tarul.cn

date +%s;  date -d @1700000000
来源：http://vej.vehdjk.com

[R71] 日期格式化
来源：http://kaf.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xpa.wangdashe.top

[R72] 等待端口就绪
来源：http://imo.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://edg.gaohongyu789.top

[R73] 分割大日志
来源：http://sip.cheryme.top

split -l 1000 big.log part_
来源：http://nvr.cqqwz.cn

[R74] 批量重命名
来源：http://plh.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ckc.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://ghs.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://apn.xuanzx.com

[R76] 使用临时文件
来源：http://jtl.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vyk.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://rbg.fktsv.cn

read -rp "请输入: " ans
来源：http://ucy.xuanzx.com

[R78] 交互式菜单
来源：http://jsv.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ded.jinghuilouyu.cn

[R79] 解析命令行选项
来源：http://iho.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mqv.c1oappe.top

[R80] 查看脚本执行耗时
来源：http://eas.hnxiangtu.top

time ./run.sh
来源：http://yse.316326.xyz

================================================================================
来源：http://ojr.cqqwz.cn

S. C / C++ 专题
来源：http://zlk.quarkkingdee.top

================================================================================
来源：http://hxb.dianchejie.cn

[S01] C：Hello World
来源：http://ard.guannengcc.top

#include <stdio.h>
来源：http://dwu.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rfs.zycfv.cn

[S02] C：变量与格式化输出
来源：http://mxy.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://kwj.jianghu66.top

[S03] C：读入整数
来源：http://ruz.wangdashe.top

int x; scanf("%d", &x);
来源：http://iuq.nwbrower.top

[S04] C：字符串复制
来源：http://irk.sxryk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wyb.dianchejie.cn

[S05] C：字符串长度
来源：http://mbg.xinyue.icu


<!-- 参考信息 -->