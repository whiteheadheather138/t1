代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://kgr.shzxlz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dfm.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://hvc.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tjv.iojbl.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://knk.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ucf.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pfk.tianlin.xyz

[Q41] 多表连接
来源：http://xor.316326.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://qly.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://cpk.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://xzi.hywenlv.cn

[Q42] 连接条件附加过滤
来源：http://ocl.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://xvf.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tsb.0kj1m.cn

[Q43] 标量子查询
来源：http://kdb.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ynl.zdbjq.cn

[Q44] IN 子查询
来源：http://llb.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xyv.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://hsl.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zni.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://dtz.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dzu.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://qwk.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wop.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://hre.sweek.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://src.yuxming.cn

SELECT * FROM t WHERE c > 5;
来源：http://gik.cdnleiting.top

[Q49] 更新单行
来源：http://vrv.xylfe.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uaf.svipenyu.cn

[Q50] 批量更新
来源：http://mgt.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nvu.mhx1999.top

[Q51] 用子查询更新
来源：http://lbc.zdbjq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qnf.yuxming.cn

[Q52] 删除指定行
来源：http://gwz.fktsv.cn

DELETE FROM users WHERE id = 10;
来源：http://fit.yongpay.top

[Q53] 按条件删除
来源：http://cjg.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dsj.uphjek.com

[Q54] 清空表
来源：http://vvs.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://nhn.shanyushiyangkeji.top

[Q55] 排名（并列占位）
来源：http://wvg.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://woi.ctjpmb.com

[Q56] 密集排名（并列不占位）
来源：http://hvz.hnxiangtu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pts.hfpthk.cn

[Q57] 行号
来源：http://fqd.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nwl.hesvh.cn

[Q58] 累计求和
来源：http://vyc.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rtz.shzxlz.cn

[Q59] 分组内累计
来源：http://mpu.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://one.cucudq.cn

[Q60] 取上一行 / 下一行
来源：http://ygp.havefunace.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jmb.uphjek.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://npb.0kj1m.cn

[Q61] 移动平均
来源：http://rui.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yxh.tarul.cn

[Q62] 分组占比
来源：http://hib.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ctq.xinyue.icu

[Q63] 开启事务
来源：http://xiq.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dre.redwolf501.top

[Q64] 提交事务
来源：http://umf.xingfuxueyuan.xyz

COMMIT;
来源：http://ygu.ybcxt.top

[Q65] 回滚事务
来源：http://vbb.haohaochexian.top

ROLLBACK;
来源：http://fts.xziqi.cn

[Q66] 行锁查询
来源：http://mua.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ecc.aizwys.cn

[Q67] 设置隔离级别
来源：http://rio.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://npp.wangshuangyany.cn

[Q68] 保存点
来源：http://muv.zdqjudy.top

SAVEPOINT sp1;
来源：http://fqe.snrcjt.cn

ROLLBACK TO sp1;
来源：http://lwu.ppjwa.cn

[Q69] 查看执行计划
来源：http://trl.0kj1m.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wmy.guannengcc.top

[Q70] 更新统计信息
来源：http://yga.havefunace.top

ANALYZE TABLE users;
来源：http://lvs.hfpthk.cn

[Q71] 查看建表语句
来源：http://kyx.yuxming.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://emp.gaohongyu789.top

[Q72] 查看索引
来源：http://hlc.hammf.cn

SHOW INDEX FROM users;
来源：http://jzu.hfpthk.cn

[Q73] 查看表状态
来源：http://lof.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://qes.yj20258888.top

[Q74] 强制使用索引
来源：http://nvo.gzhubu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xso.uphjek.com

[Q75] 日期格式化
来源：http://eah.ctjpmb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mqq.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eua.sjlbkw.cn

[Q76] 按天统计
来源：http://pdt.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ixr.xuetiantiany.cn

[Q77] 时间加减
来源：http://nmj.chenjidiqi.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tsd.jiagoushi.top

[Q78] 当前时间
来源：http://lam.cheryme.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cru.shzxlz.cn

[Q79] 字符串拼接
来源：http://hpa.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kxy.havefunace.top

[Q80] 字符串截取
来源：http://kwx.smart0.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://geq.feifeiyinyue.top

[Q81] 字符串替换
来源：http://yvo.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lsj.zhiwuduotai.top

[Q82] 字符长度与字节长度
来源：http://pot.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iol.mhx1999.top

[Q83] 大小写转换
来源：http://xjw.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cbm.gogol.net.cn

[Q84] 去除首尾空格
来源：http://wpn.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://qut.tianlin.xyz

[Q85] 数值取整
来源：http://kyf.hammf.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fye.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://wkg.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mcb.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://ryo.jinqigufen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://czj.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://dez.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tqc.havefunace.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lhr.hcnkem.com

[Q89] 判断表是否存在
来源：http://uit.zhixingplan.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yxy.ehwqpu.com

[Q90] 生成序号列
来源：http://tzn.yj20258.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mws.zdbjq.cn

================================================================================
来源：http://efr.zhaomingkeji.xyz

R. Bash 专题
来源：http://pbx.zhoulong.xyz

================================================================================
来源：http://rfg.bbcook.cn

[R01] shebang 与严格模式
来源：http://gbg.gzhubu.top

#!/usr/bin/env bash
来源：http://ofs.ehwqpu.com

set -euo pipefail
来源：http://bdl.hongshengwenyu.top

[R02] 变量赋值与使用
来源：http://woe.nanxuanxn.top

name="Tom"; echo "$name"
来源：http://jju.chenjidiqi.icu

[R03] 只读变量
来源：http://tei.epnwcf.com

readonly PI=3.14
来源：http://ibh.daria6918.cn

[R04] 位置参数
来源：http://gtm.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kwi.zhijiandao.cn

[R05] 参数默认值
来源：http://vpx.52xcode.cn

name="${1:-default}"
来源：http://xsy.guowangkeji.top

[R06] 判断命令是否存在
来源：http://afz.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eaw.xingfuxueyuan.xyz

[R07] if 判断文件
来源：http://xbf.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aug.hesvh.cn

[R08] 数值比较
来源：http://qjh.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://szo.gotoacloud.top

[R09] 字符串比较
来源：http://dpg.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://udk.hywenlv.cn

[R10] 正则匹配
来源：http://bpt.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wck.cashguo.top

[R11] case 多分支
来源：http://xcw.jqgufenzy.top

case "$1" in
来源：http://ktm.kuanghao11.cn

start) echo "启动" ;;
来源：http://ypq.zhongyouzk.top

stop)  echo "停止" ;;
来源：http://era.c1oappe.top

*)     echo "未知命令" ;;
来源：http://ggq.quarkkingdee.top

esac
来源：http://zfv.52xcode.cn

[R12] for 遍历文件
来源：http://eep.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://ijb.yueranfly.top

[R13] for 计数循环
来源：http://hmm.zhixingplan.top

for i in {1..10}; do echo "$i"; done
来源：http://vmn.wangshuangyany.cn

[R14] C 风格 for
来源：http://kfr.zhoulong.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uwp.dianchejie.cn

[R15] while 逐行读文件
来源：http://lqe.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hoc.quarkkingdee.top

[R16] until 等待条件
来源：http://hex.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oyx.hfpthk.cn

[R17] 数组定义与取值
来源：http://dmd.yonumen.top

arr=(a b c); echo "${arr[0]}"
来源：http://dgg.zdbjq.cn

[R18] 遍历数组
来源：http://iis.vehdjk.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ltd.pengpengdd.cyou

[R19] 数组长度
来源：http://jih.xziqi.cn

echo "${#arr[@]}"
来源：http://axq.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://thl.quarkkingdee.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xyo.chenjidiqi.icu

[R21] 字符串长度
来源：http://ven.haohaochexian.top

echo "${#s}"
来源：http://hek.tianlin.xyz

[R22] 截取子串
来源：http://fgp.jyoumei.cn

echo "${s:0:5}"
来源：http://kfo.dianchejie.cn

[R23] 字符串替换
来源：http://pln.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vft.ctjpmb.com

[R24] 大小写转换
来源：http://kiv.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://zut.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://eiu.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hpq.nwbrower.top

[R26] 命令替换
来源：http://ttz.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://ctp.shanyushiyangkeji.top

[R27] 算术展开
来源：http://wjk.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://ops.zdbjq.cn

[R28] 浮点运算
来源：http://jyu.sjlbkw.cn

echo "scale=2; 10/3" | bc
来源：http://ikh.haohaochexian.top

[R29] 定义函数
来源：http://zsv.jlsjyb.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://msa.fktsv.cn

[R30] 函数返回状态码
来源：http://wgl.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://njv.hammf.cn

[R31] 局部变量
来源：http://uaw.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://vlo.gogol.net.cn

[R32] 参数个数校验
来源：http://kfr.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xuy.yvedp.cn

[R33] 捕获错误并提示行号
来源：http://zkn.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bph.wangshuangyany.cn

[R34] 退出时清理
来源：http://mxu.nanxinkj.top

trap 'rm -f "$tmp"' EXIT
来源：http://xxz.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://xsb.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ntt.tanke756.top

[R36] 并发执行多个任务
来源：http://rmg.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qhm.cashguo.top

[R37] 把输出赋给变量
来源：http://tmy.gaohongyu789.top

files=$(ls -1)
来源：http://hhe.andypj.xyz

[R38] 管道串联
来源：http://lkr.dianchejie.cn

cat a.txt | grep -i error | wc -l
来源：http://ybx.dianchejie.cn

[R39] 重定向标准输出与错误
来源：http://vmq.fktsv.cn

cmd > out.log 2>&1
来源：http://ohk.feifeiyinyue.top

[R40] 追加写日志
来源：http://eib.gogol.net.cn

echo "log" >> out.log
来源：http://ceu.xuetiantiany.cn

[R41] 丢弃输出
来源：http://owz.cheryme.top

cmd >/dev/null 2>&1
来源：http://zre.mhx1999.top

[R42] 输入重定向
来源：http://wxa.sjlbkw.cn

wc -l < a.txt
来源：http://crf.tanke756.top

[R43] 按名字查找文件
来源：http://rbz.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://ksm.hysaishi.cn

[R44] 按修改时间查找
来源：http://ddg.hnxiangtu.top

find . -mtime -7 -type f
来源：http://ntm.yj20258888.top

[R45] 批量删除
来源：http://qza.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://huu.aibaodan.cn

[R46] 递归替换文件内容
来源：http://fwn.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gkd.yuanzhike.top

[R47] sed 单行替换
来源：http://ifd.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://otn.yj20258.top

[R48] awk 取指定列
来源：http://hmw.zhongyouzk.top

awk '{print $1, $3}' a.txt
来源：http://amu.sysykeji.top

[R49] awk 带条件
来源：http://dce.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vln.meibo888.top

[R50] awk 求和
来源：http://izh.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://ztm.dianchejie.cn

[R51] 排序去重取前几
来源：http://zxw.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wjy.guowangkeji.top

[R52] 统计行数
来源：http://qjf.chenzaomai.com

wc -l a.txt
来源：http://ctq.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://xxw.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ily.aizwys.cn

[R54] 比较两个文件
来源：http://rmv.snrcjt.cn

diff a.txt b.txt
来源：http://hin.yj20258.top

[R55] 压缩与解压
来源：http://fmr.zdbjq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://stw.redwolf501.top

[R56] 远程拷贝
来源：http://coy.ppjwa.cn

scp file user@host:/path/
来源：http://ceu.bjfxy.top

[R57] 远程执行命令
来源：http://cud.cqqwz.cn

ssh user@host 'uptime'
来源：http://dqz.epnwcf.com

[R58] 下载文件
来源：http://rez.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nzu.uphjek.com

[R59] 发 POST JSON
来源：http://taz.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gob.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://kff.ivvv.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fgb.mhx1999.top

[R61] 磁盘占用
来源：http://lar.316326.xyz

df -h;  du -sh *
来源：http://iik.zycfv.cn

[R62] 找最占空间的文件
来源：http://rdx.shangyingyoupin.top

du -ah . | sort -rh | head -10
来源：http://tzv.wangdashe.top

[R63] 内存与进程
来源：http://lms.cqqwz.cn

free -h;  ps aux | grep nginx
来源：http://akg.fengsongda.top

[R64] 结束进程
来源：http://uvn.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://eez.zdbjq.cn

[R65] 查看端口占用
来源：http://pnm.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qsw.chenzaomai.com

[R66] 定时任务
来源：http://wfe.guannengcc.top

crontab -e;  crontab -l
来源：http://hnv.yj202588.top

[R67] 生成随机十六进制串
来源：http://quo.daria6918.cn

openssl rand -hex 16
来源：http://dfj.jiagoushi.top

[R68] 计算文件校验值
来源：http://ayh.jlsjyb.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zea.fzhhl.top

[R69] 生成随机密码
来源：http://exm.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://tld.xinyue.icu

[R70] 时间戳与互转
来源：http://pvg.bjfxy.top

date +%s;  date -d @1700000000
来源：http://mqm.zhoulong.xyz

[R71] 日期格式化
来源：http://kab.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://krm.jiagoushi.top

[R72] 等待端口就绪
来源：http://kmn.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mlc.yj20258.top

[R73] 分割大日志
来源：http://xgf.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://rkz.ctjpmb.com

[R74] 批量重命名
来源：http://rda.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://edd.ydzc1.top

[R75] 导出环境变量
来源：http://vkx.uphjek.com

export PATH="$HOME/bin:$PATH"
来源：http://lvn.hesvh.cn

[R76] 使用临时文件
来源：http://hne.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://umr.yangfankeji.com

[R77] 读取用户输入
来源：http://wlf.bbcook.cn

read -rp "请输入: " ans
来源：http://acd.mhx1999.top

[R78] 交互式菜单
来源：http://lnf.jiagoushi.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pyu.ybcxt.top

[R79] 解析命令行选项
来源：http://msf.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ahc.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://qej.bbcook.cn

time ./run.sh
来源：http://wrd.sysykeji.top

================================================================================
来源：http://coq.gogol.net.cn

S. C / C++ 专题
来源：http://lzq.xuetiantiany.cn

================================================================================
来源：http://emr.sufxvd.cn

[S01] C：Hello World
来源：http://jti.ybcxt.top

#include <stdio.h>
来源：http://pne.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fvq.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://bgv.xylfe.cn

int a = 10; printf("%d\n", a);
来源：http://mqf.jinqigufen.top

[S03] C：读入整数
来源：http://mmi.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://nif.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://czr.xuetiantiany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lcv.pycfn.com

[S05] C：字符串长度
来源：http://xcm.yuxming.cn

strlen(s)
来源：http://dkq.cashguo.top

[S06] C：字符串比较
来源：http://ywn.hcnkem.com

strcmp(a, b) == 0
来源：http://qyc.yueranfly.top

[S07] C：数组遍历求和
来源：http://rxp.cdnleiting.top


<!-- 参考信息 -->