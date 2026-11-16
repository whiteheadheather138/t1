代发 wailian999

[Q33] 多列分组
来源：http://wbh.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://chu.zhijiandao.cn

[Q34] 每组取第一条
来源：http://tgr.zhixingplan.top

SELECT * FROM (
来源：http://ylb.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nxw.c1oappe.top

) t WHERE rn = 1;
来源：http://jso.vqdsnc.cn

[Q35] 内连接
来源：http://tfu.cucudq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ecl.zhaomingkeji.xyz

[Q36] 左连接
来源：http://kto.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zsc.0kj1m.cn

[Q37] 右连接
来源：http://wqt.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mge.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://cvg.nanxinkj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cyd.jlsjyb.cn

[Q39] 自连接（查上下级）
来源：http://poz.xinyue.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://awh.nanxuanxn.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://clh.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fyw.haohaochexian.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mjg.gotoacloud.top

[Q41] 多表连接
来源：http://lef.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://jxw.daxiang520.top

JOIN users u ON u.id = o.user_id
来源：http://mmw.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://tzl.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://cwu.cqqwz.cn

SELECT u.name, o.amount FROM users u
来源：http://vtd.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nla.wangshuangyany.cn

[Q43] 标量子查询
来源：http://mrs.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kps.ywan-chungtsiang.top

[Q44] IN 子查询
来源：http://wmt.fktsv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jdk.meibo888.top

[Q45] EXISTS 判断存在
来源：http://tsy.cucudq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sgw.hongshengwenyu.top

[Q46] NOT EXISTS 判断不存在
来源：http://tor.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hra.jyoumei.cn

[Q47] 与平均值比较
来源：http://jwp.yj20258.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gyn.hywenlv.cn

[Q48] CTE 公用表表达式
来源：http://fyw.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pmm.yuxming.cn

SELECT * FROM t WHERE c > 5;
来源：http://qrt.hysaishi.cn

[Q49] 更新单行
来源：http://kzh.jqgufenzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lta.316326.xyz

[Q50] 批量更新
来源：http://vzv.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oui.zhongyouzk.top

[Q51] 用子查询更新
来源：http://rwj.pycfn.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yqi.cqqwz.cn

[Q52] 删除指定行
来源：http://ync.sweek.top

DELETE FROM users WHERE id = 10;
来源：http://jwz.vqdsnc.cn

[Q53] 按条件删除
来源：http://dfm.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xmd.ybcxt.top

[Q54] 清空表
来源：http://ffo.fzhhl.top

TRUNCATE TABLE logs;
来源：http://wtw.yongpay.top

[Q55] 排名（并列占位）
来源：http://oxd.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://knh.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://vwh.zhengqikj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vri.ehwqpu.com

[Q57] 行号
来源：http://omg.9152youxi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://frk.uphjek.com

[Q58] 累计求和
来源：http://vqd.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://unr.xziqi.cn

[Q59] 分组内累计
来源：http://jkz.zhoulong.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://auc.tarul.cn

[Q60] 取上一行 / 下一行
来源：http://spy.jiagoushi.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tcc.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qva.fengsongda.top

[Q61] 移动平均
来源：http://olp.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wmx.jiagoushi.top

[Q62] 分组占比
来源：http://hed.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uem.smart0.xyz

[Q63] 开启事务
来源：http://fky.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hqr.jinghuilouyu.cn

[Q64] 提交事务
来源：http://rpe.daxiang520.top

COMMIT;
来源：http://wcq.fehbvm.com

[Q65] 回滚事务
来源：http://uox.tian-w.cn

ROLLBACK;
来源：http://fqq.fktsv.cn

[Q66] 行锁查询
来源：http://pcu.pengpengdd.cyou

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rmd.chenjidiqi.icu

[Q67] 设置隔离级别
来源：http://ofu.hcnkem.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uzs.pycfn.com

[Q68] 保存点
来源：http://kxm.zdqjudy.top

SAVEPOINT sp1;
来源：http://dwa.hammf.cn

ROLLBACK TO sp1;
来源：http://ahu.hysaishi.cn

[Q69] 查看执行计划
来源：http://tnf.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hon.pengpengdd.cyou

[Q70] 更新统计信息
来源：http://clo.guowangkeji.top

ANALYZE TABLE users;
来源：http://dxk.ydzc1.top

[Q71] 查看建表语句
来源：http://ace.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hte.hysaishi.cn

[Q72] 查看索引
来源：http://xsf.52xcode.cn

SHOW INDEX FROM users;
来源：http://vjo.smart0.xyz

[Q73] 查看表状态
来源：http://hyp.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ypn.gaohongyu789.top

[Q74] 强制使用索引
来源：http://mhs.9152youxi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ikr.wangdashe.top

[Q75] 日期格式化
来源：http://pgl.gaohongyu789.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hbd.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rfb.9152youxi.cn

[Q76] 按天统计
来源：http://ood.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ubj.daria6918.cn

[Q77] 时间加减
来源：http://mhv.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://svf.ctjpmb.com

[Q78] 当前时间
来源：http://tlr.gotoacloud.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rnv.wangdashe.top

[Q79] 字符串拼接
来源：http://kfj.c1oappe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jub.ydzc1.top

[Q80] 字符串截取
来源：http://xlx.yvedp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sri.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://qdo.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oph.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://wtg.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hjk.zycfv.cn

[Q83] 大小写转换
来源：http://chb.jianghu66.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zed.gotoacloud.top

[Q84] 去除首尾空格
来源：http://wzi.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://ann.kuanghao11.cn

[Q85] 数值取整
来源：http://iql.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://niv.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://zho.yueranfly.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yhh.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://gwv.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eqy.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://tpp.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rwa.hcnkem.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fhv.aizwys.cn

[Q89] 判断表是否存在
来源：http://xrf.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kkf.52xcode.cn

[Q90] 生成序号列
来源：http://zco.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://czr.iojbl.cn

================================================================================
来源：http://tze.epnwcf.com

R. Bash 专题
来源：http://rrb.hysaishi.cn

================================================================================
来源：http://mie.fzhhl.top

[R01] shebang 与严格模式
来源：http://fnh.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://ghl.jqgfzy.top

set -euo pipefail
来源：http://mlf.snrcjt.cn

[R02] 变量赋值与使用
来源：http://men.jianghu66.top

name="Tom"; echo "$name"
来源：http://jva.dashuyun.cn

[R03] 只读变量
来源：http://vqj.smart0.xyz

readonly PI=3.14
来源：http://ruw.jinqigfzy.top

[R04] 位置参数
来源：http://zxs.bjfxy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gky.shzxlz.cn

[R05] 参数默认值
来源：http://uqs.shanyushiyangkeji.top

name="${1:-default}"
来源：http://fau.gzhubu.top

[R06] 判断命令是否存在
来源：http://bvi.daxiang520.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cyt.jinqigfzy.top

[R07] if 判断文件
来源：http://gkm.gzhubu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tkh.hfpthk.cn

[R08] 数值比较
来源：http://vrx.yvedp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jjj.ctjpmb.com

[R09] 字符串比较
来源：http://hks.zhengqikj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lkk.gotoacloud.top

[R10] 正则匹配
来源：http://svh.gogol.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jnj.c1oappe.top

[R11] case 多分支
来源：http://pwr.52xcode.cn

case "$1" in
来源：http://pjz.smart0.xyz

start) echo "启动" ;;
来源：http://qfz.hammf.cn

stop)  echo "停止" ;;
来源：http://urn.bjfxy.top

*)     echo "未知命令" ;;
来源：http://eoq.wangdashe.top

esac
来源：http://jqs.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://pdi.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://vib.c1oappe.top

[R13] for 计数循环
来源：http://kzi.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://zyf.bbcook.cn

[R14] C 风格 for
来源：http://oni.tarul.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xkm.yongpay.top

[R15] while 逐行读文件
来源：http://neo.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sff.yuanzhike.top

[R16] until 等待条件
来源：http://laf.jqgufenzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dqw.yuanzhike.top

[R17] 数组定义与取值
来源：http://axk.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sld.smart0.xyz

[R18] 遍历数组
来源：http://etb.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vbw.hnqzz.top

[R19] 数组长度
来源：http://upa.ivvv.top

echo "${#arr[@]}"
来源：http://edv.fehbvm.com

[R20] 关联数组（字典）
来源：http://que.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bmr.tarul.cn

[R21] 字符串长度
来源：http://oah.ehwqpu.com

echo "${#s}"
来源：http://zld.ehwqpu.com

[R22] 截取子串
来源：http://axf.yongpay.top

echo "${s:0:5}"
来源：http://okx.yuxming.cn

[R23] 字符串替换
来源：http://bda.tanke756.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bpl.ctjpmb.com

[R24] 大小写转换
来源：http://gpm.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://hzo.xuanzx.com

[R25] 去后缀 / 去前缀
来源：http://cvp.zdbjq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://snl.aizwys.cn

[R26] 命令替换
来源：http://rde.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://zfi.hfpthk.cn

[R27] 算术展开
来源：http://ake.jyoumei.cn

echo $((1 + 2 * 3))
来源：http://bwi.zhengqikj.top

[R28] 浮点运算
来源：http://ira.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://wiw.aibaodan.cn

[R29] 定义函数
来源：http://dgs.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fxg.jyoumei.cn

[R30] 函数返回状态码
来源：http://ezw.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://itx.fehbvm.com

[R31] 局部变量
来源：http://bwf.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://fsl.cashguo.top

[R32] 参数个数校验
来源：http://kgd.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tjs.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://yzt.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nbr.jqgfzy.top

[R34] 退出时清理
来源：http://ipc.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uzi.sweek.top

[R35] 后台执行并等待
来源：http://fck.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://obd.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://ocg.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zmc.redwolf501.top

[R37] 把输出赋给变量
来源：http://bdt.redwolf501.top

files=$(ls -1)
来源：http://dcu.gotoacloud.top

[R38] 管道串联
来源：http://hzg.zhaomingkeji.xyz

cat a.txt | grep -i error | wc -l
来源：http://ldq.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://jtm.yongpay.top

cmd > out.log 2>&1
来源：http://bxk.zdbjq.cn

[R40] 追加写日志
来源：http://evl.jqgfzy.top

echo "log" >> out.log
来源：http://zuo.wangshuangyany.cn

[R41] 丢弃输出
来源：http://qkk.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://gwt.jianghu66.top

[R42] 输入重定向
来源：http://jaz.yj202588.top

wc -l < a.txt
来源：http://xkz.vehdjk.com

[R43] 按名字查找文件
来源：http://gcz.yanxiufei.cn

find . -name "*.log" -type f
来源：http://zwg.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://sgw.zhixingplan.top

find . -mtime -7 -type f
来源：http://xpd.fengsongda.top

[R45] 批量删除
来源：http://gjb.aizwys.cn

find . -name "*.tmp" -delete
来源：http://mic.chenzaomai.com

[R46] 递归替换文件内容
来源：http://jet.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://snl.haohaochexian.top

[R47] sed 单行替换
来源：http://fli.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://nvv.zycfv.cn

[R48] awk 取指定列
来源：http://etp.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://dve.feifeiyinyue.top

[R49] awk 带条件
来源：http://qgh.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iwn.kuanghao11.cn

[R50] awk 求和
来源：http://yli.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://dyx.chenzaomai.com

[R51] 排序去重取前几
来源：http://wsl.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://imp.9152youxi.cn

[R52] 统计行数
来源：http://zke.chenlongwang.top

wc -l a.txt
来源：http://akw.gzhubu.top

[R53] 查看文件头与实时尾
来源：http://skm.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wzp.nanxinkj.top

[R54] 比较两个文件
来源：http://wqi.sweek.top

diff a.txt b.txt
来源：http://xsy.xuanzx.com

[R55] 压缩与解压
来源：http://cgh.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ito.cashguo.top

[R56] 远程拷贝
来源：http://wtp.jinghuilouyu.cn

scp file user@host:/path/
来源：http://ydf.zhiwuduotai.top

[R57] 远程执行命令
来源：http://fuk.c1oappe.top

ssh user@host 'uptime'
来源：http://fbm.yj202588.top

[R58] 下载文件
来源：http://skm.gaohongyu789.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://phg.epnwcf.com

[R59] 发 POST JSON
来源：http://cqg.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uil.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://dgk.yongpay.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wfo.zdbjq.cn

[R61] 磁盘占用
来源：http://tet.jlsjyb.cn

df -h;  du -sh *
来源：http://tcu.smart0.xyz

[R62] 找最占空间的文件
来源：http://uws.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://bne.tianlin.xyz

[R63] 内存与进程
来源：http://srl.hammf.cn

free -h;  ps aux | grep nginx
来源：http://ngm.fktsv.cn

[R64] 结束进程
来源：http://exx.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://tug.zdqjudy.top

[R65] 查看端口占用
来源：http://wuk.hysaishi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lsh.vehdjk.com

[R66] 定时任务
来源：http://kvn.nanxuanxn.top

crontab -e;  crontab -l
来源：http://edv.hammf.cn

[R67] 生成随机十六进制串
来源：http://knj.snrcjt.cn

openssl rand -hex 16
来源：http://lol.yuxming.cn

[R68] 计算文件校验值
来源：http://pod.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://atw.dashuyun.cn

[R69] 生成随机密码
来源：http://bmc.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://bai.aibaodan.cn

[R70] 时间戳与互转
来源：http://fnf.uphjek.com

date +%s;  date -d @1700000000
来源：http://lvm.316326.xyz

[R71] 日期格式化
来源：http://ibt.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pwc.svipenyu.cn

[R72] 等待端口就绪
来源：http://loq.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ozc.hfpthk.cn

[R73] 分割大日志
来源：http://epn.haohaochexian.top

split -l 1000 big.log part_
来源：http://cdb.birdmap.top

[R74] 批量重命名
来源：http://akn.jinghuilouyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yry.yj202588.top

[R75] 导出环境变量
来源：http://tnt.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://vrw.fehbvm.com

[R76] 使用临时文件
来源：http://aws.kuanghao11.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bjm.316326.xyz

[R77] 读取用户输入
来源：http://bct.sxryk.cn

read -rp "请输入: " ans
来源：http://pma.chenjidiqi.icu

[R78] 交互式菜单
来源：http://dnl.guowangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kao.havefunace.top

[R79] 解析命令行选项
来源：http://xge.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://urf.shanyushiyangkeji.top

[R80] 查看脚本执行耗时
来源：http://rug.daxiang520.top

time ./run.sh
来源：http://mvi.chenzaomai.com

================================================================================
来源：http://rhf.fanxiaobao.xyz

S. C / C++ 专题
来源：http://jki.ybcxt.top

================================================================================
来源：http://opv.xylfe.cn

[S01] C：Hello World
来源：http://aug.sxryk.cn

#include <stdio.h>
来源：http://mcw.hnxiangtu.top


<!-- 参考信息 -->