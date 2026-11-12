代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://frt.wangdashe.top

) t WHERE rn = 1;
来源：http://xpp.andypj.xyz

[Q35] 内连接
来源：http://qix.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qrp.tanke756.top

[Q36] 左连接
来源：http://bjd.sufxvd.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lhg.jinqigufen.top

[Q37] 右连接
来源：http://nac.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qxf.fanxiaobao.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://ezb.tian-w.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kal.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://pbk.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ere.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cwl.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yot.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://orq.yongpay.top

[Q41] 多表连接
来源：http://fsb.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://itn.jinyuanbaomall.cn

JOIN users u ON u.id = o.user_id
来源：http://hut.tianlin.xyz

JOIN products p ON p.id = o.product_id;
来源：http://mgx.yj20258888.top

[Q42] 连接条件附加过滤
来源：http://odk.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://kdi.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fxn.hywenlv.cn

[Q43] 标量子查询
来源：http://pzh.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eod.xuanzx.com

[Q44] IN 子查询
来源：http://quw.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fyt.nwbrower.top

[Q45] EXISTS 判断存在
来源：http://rxg.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wzq.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://irz.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sik.ybcxt.top

[Q47] 与平均值比较
来源：http://btc.cashguo.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hkf.nanxuanxn.top

[Q48] CTE 公用表表达式
来源：http://iku.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tyt.hcnkem.com

SELECT * FROM t WHERE c > 5;
来源：http://dtt.shuidangran.top

[Q49] 更新单行
来源：http://vbm.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rbd.sysykeji.top

[Q50] 批量更新
来源：http://fai.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://emt.nanxinkj.top

[Q51] 用子查询更新
来源：http://eal.shzxlz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xgh.yanxiufei.cn

[Q52] 删除指定行
来源：http://grf.ppjwa.cn

DELETE FROM users WHERE id = 10;
来源：http://iym.ehwqpu.com

[Q53] 按条件删除
来源：http://qce.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://shh.zdqjudy.top

[Q54] 清空表
来源：http://ngk.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://yye.nanxuanxn.top

[Q55] 排名（并列占位）
来源：http://dwh.hysaishi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://svl.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://obn.chenlongwang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xlp.fengsongda.top

[Q57] 行号
来源：http://vgq.yvedp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lhr.hywenlv.cn

[Q58] 累计求和
来源：http://rmk.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://txo.vqdsnc.cn

[Q59] 分组内累计
来源：http://dpq.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cgi.fzhhl.top

[Q60] 取上一行 / 下一行
来源：http://ped.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bbb.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aip.jinqigfzy.top

[Q61] 移动平均
来源：http://nzu.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kvl.zhijiandao.cn

[Q62] 分组占比
来源：http://ivg.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xqg.daria6918.cn

[Q63] 开启事务
来源：http://iry.nwbrower.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rsp.zdqjudy.top

[Q64] 提交事务
来源：http://gmr.jlsjyb.cn

COMMIT;
来源：http://tjg.xinyue.icu

[Q65] 回滚事务
来源：http://rfg.jinqigufen.top

ROLLBACK;
来源：http://slo.zhijiandao.cn

[Q66] 行锁查询
来源：http://vtd.chenzaomai.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ydc.nwbrower.top

[Q67] 设置隔离级别
来源：http://ava.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://enk.cheryme.top

[Q68] 保存点
来源：http://wyo.jinqigufen.top

SAVEPOINT sp1;
来源：http://cjr.havefunace.top

ROLLBACK TO sp1;
来源：http://rpo.zdqjudy.top

[Q69] 查看执行计划
来源：http://uvq.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dsx.fzhhl.top

[Q70] 更新统计信息
来源：http://ewb.yuxming.cn

ANALYZE TABLE users;
来源：http://fyv.zhijiandao.cn

[Q71] 查看建表语句
来源：http://gco.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kpn.fehbvm.com

[Q72] 查看索引
来源：http://mpf.sysykeji.top

SHOW INDEX FROM users;
来源：http://vsr.feifeiyinyue.top

[Q73] 查看表状态
来源：http://avc.yuxming.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wer.chenzaomai.com

[Q74] 强制使用索引
来源：http://ngs.ctjpmb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fjh.yfazqb.com

[Q75] 日期格式化
来源：http://fqj.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rzz.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fjz.yueranfly.top

[Q76] 按天统计
来源：http://unr.shanyushiyangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kjr.fengsongda.top

[Q77] 时间加减
来源：http://yzf.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vsv.andypj.xyz

[Q78] 当前时间
来源：http://cde.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zpk.dianchejie.cn

[Q79] 字符串拼接
来源：http://lyf.yueranfly.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cby.yj202588.top

[Q80] 字符串截取
来源：http://hap.jlsjyb.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kgi.andypj.xyz

[Q81] 字符串替换
来源：http://qcw.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jet.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://ghw.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://btn.zdbjq.cn

[Q83] 大小写转换
来源：http://csx.tian-w.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://epd.jlsjyb.cn

[Q84] 去除首尾空格
来源：http://jix.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://idr.fehbvm.com

[Q85] 数值取整
来源：http://ibb.shuidangran.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jdn.jinqigufen.top

[Q86] 读取 JSON 字段
来源：http://tqt.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kjq.ehwqpu.com

[Q87] JSON 字段做条件
来源：http://xai.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lxu.yuxming.cn

[Q88] 行转列（条件聚合）
来源：http://evn.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tpp.andypj.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jpl.yj202588.top

[Q89] 判断表是否存在
来源：http://zhe.shzxlz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ryy.gaohongyu789.top

[Q90] 生成序号列
来源：http://apz.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vym.snrcjt.cn

================================================================================
来源：http://xmb.jqgufenzy.top

R. Bash 专题
来源：http://ugc.pycfn.com

================================================================================
来源：http://qas.bbcook.cn

[R01] shebang 与严格模式
来源：http://yiq.hfpthk.cn

#!/usr/bin/env bash
来源：http://fpa.smart0.xyz

set -euo pipefail
来源：http://ndn.ehwqpu.com

[R02] 变量赋值与使用
来源：http://ghf.aibaodan.cn

name="Tom"; echo "$name"
来源：http://xqc.yongpay.top

[R03] 只读变量
来源：http://kdh.pycfn.com

readonly PI=3.14
来源：http://ije.daxiang520.top

[R04] 位置参数
来源：http://cgi.0kj1m.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kzo.jqgufenzy.top

[R05] 参数默认值
来源：http://qoo.gotoacloud.top

name="${1:-default}"
来源：http://xpl.guannengcc.top

[R06] 判断命令是否存在
来源：http://ipm.zhiwuduotai.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gvw.fzhhl.top

[R07] if 判断文件
来源：http://ymh.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zlw.zhongyouzk.top

[R08] 数值比较
来源：http://hsp.jiagoushi.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fhs.hnxiangtu.top

[R09] 字符串比较
来源：http://mbi.zhijiandao.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://foi.yongpay.top

[R10] 正则匹配
来源：http://fwf.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nrh.sxryk.cn

[R11] case 多分支
来源：http://adr.haohaochexian.top

case "$1" in
来源：http://slv.52xcode.cn

start) echo "启动" ;;
来源：http://qzh.yuanzhike.top

stop)  echo "停止" ;;
来源：http://lol.yangfankeji.com

*)     echo "未知命令" ;;
来源：http://jiu.52xcode.cn

esac
来源：http://wof.fehbvm.com

[R12] for 遍历文件
来源：http://oto.aizwys.cn

for f in *.txt; do echo "$f"; done
来源：http://xzp.mhx1999.top

[R13] for 计数循环
来源：http://sie.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://nyv.andypj.xyz

[R14] C 风格 for
来源：http://wgf.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tsv.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://ciq.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bfd.sysykeji.top

[R16] until 等待条件
来源：http://hpm.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ela.ydjk.org.cn

[R17] 数组定义与取值
来源：http://agx.zhengqikj.top

arr=(a b c); echo "${arr[0]}"
来源：http://qlk.gotoacloud.top

[R18] 遍历数组
来源：http://zqy.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xqt.dianchejie.cn

[R19] 数组长度
来源：http://kgi.wangdashe.top

echo "${#arr[@]}"
来源：http://qtf.shanyushiyangkeji.top

[R20] 关联数组（字典）
来源：http://jru.daria6918.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://akm.shzxlz.cn

[R21] 字符串长度
来源：http://vkp.shanyushiyangtech.top

echo "${#s}"
来源：http://ecp.jinqigufen.top

[R22] 截取子串
来源：http://aiz.guannengcc.top

echo "${s:0:5}"
来源：http://kup.jinqigfzy.top

[R23] 字符串替换
来源：http://tpc.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mtl.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://vqr.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://jsx.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://wwc.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://wsy.chenlongwang.top

[R26] 命令替换
来源：http://zko.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://dab.yvedp.cn

[R27] 算术展开
来源：http://kha.nwbrower.top

echo $((1 + 2 * 3))
来源：http://bkq.jqgfzy.top

[R28] 浮点运算
来源：http://jru.jinyuanbaomall.cn

echo "scale=2; 10/3" | bc
来源：http://qcv.guannengcc.top

[R29] 定义函数
来源：http://mzo.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pgs.aizwys.cn

[R30] 函数返回状态码
来源：http://jed.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://hvh.52xcode.cn

[R31] 局部变量
来源：http://fim.xingfuxueyuan.xyz

f() { local x=1; echo "$x"; }
来源：http://erb.guannengcc.top

[R32] 参数个数校验
来源：http://wmv.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yzn.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://hya.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wpi.yonumen.top

[R34] 退出时清理
来源：http://snx.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://lng.ehwqpu.com

[R35] 后台执行并等待
来源：http://xjd.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://djf.nwbrower.top

[R36] 并发执行多个任务
来源：http://yto.daria6918.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eyd.daxiang520.top

[R37] 把输出赋给变量
来源：http://ozy.pycfn.com

files=$(ls -1)
来源：http://vnn.jianghu66.top

[R38] 管道串联
来源：http://xlc.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://dmy.vqdsnc.cn

[R39] 重定向标准输出与错误
来源：http://eec.yvedp.cn

cmd > out.log 2>&1
来源：http://ieq.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://cvb.dianchejie.cn

echo "log" >> out.log
来源：http://gwr.zycfv.cn

[R41] 丢弃输出
来源：http://ezw.mhx1999.top

cmd >/dev/null 2>&1
来源：http://zos.aibaodan.cn

[R42] 输入重定向
来源：http://qws.zhoulong.xyz

wc -l < a.txt
来源：http://bjj.sweek.top

[R43] 按名字查找文件
来源：http://grk.gzhubu.top

find . -name "*.log" -type f
来源：http://lka.birdmap.top

[R44] 按修改时间查找
来源：http://khn.yonumen.top

find . -mtime -7 -type f
来源：http://hbo.shanyushiyangkeji.top

[R45] 批量删除
来源：http://cta.mhx1999.top

find . -name "*.tmp" -delete
来源：http://ucc.yj20258888.top

[R46] 递归替换文件内容
来源：http://jpm.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hnc.hfpthk.cn

[R47] sed 单行替换
来源：http://gnq.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://thk.cdnleiting.top

[R48] awk 取指定列
来源：http://yai.zdbjq.cn

awk '{print $1, $3}' a.txt
来源：http://puf.xinyue.icu

[R49] awk 带条件
来源：http://gln.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://emg.yongpay.top

[R50] awk 求和
来源：http://mvm.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bbn.zhixingplan.top

[R51] 排序去重取前几
来源：http://aul.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://myn.gaohongyu789.top

[R52] 统计行数
来源：http://abu.zdbjq.cn

wc -l a.txt
来源：http://jrl.jinghuilouyu.cn

[R53] 查看文件头与实时尾
来源：http://vld.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lxu.hnqzz.top

[R54] 比较两个文件
来源：http://gng.yanxiufei.cn

diff a.txt b.txt
来源：http://uym.kuanghao11.cn

[R55] 压缩与解压
来源：http://bgj.zdbjq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mgv.yanxiufei.cn

[R56] 远程拷贝
来源：http://vqy.nanxuanxn.top

scp file user@host:/path/
来源：http://ikg.zycfv.cn

[R57] 远程执行命令
来源：http://wfm.hnqzz.top

ssh user@host 'uptime'
来源：http://avb.pengpengdd.cyou

[R58] 下载文件
来源：http://pqj.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lqv.zhengqikj.top

[R59] 发 POST JSON
来源：http://icl.sufxvd.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iui.fzhhl.top

[R60] 只看 HTTP 状态码
来源：http://kge.cdnleiting.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ebr.zhijiandao.cn

[R61] 磁盘占用
来源：http://jht.ivvv.top

df -h;  du -sh *
来源：http://fzq.fehbvm.com

[R62] 找最占空间的文件
来源：http://bjk.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://arw.svipenyu.cn

[R63] 内存与进程
来源：http://tci.yfazqb.com

free -h;  ps aux | grep nginx
来源：http://oxg.jinqigufen.top

[R64] 结束进程
来源：http://lbc.svipenyu.cn

kill -9 $(pgrep -f app.py)
来源：http://ssp.sufxvd.cn

[R65] 查看端口占用
来源：http://omw.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lag.fengsongda.top

[R66] 定时任务
来源：http://jrp.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://yfd.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://vvv.yanxiufei.cn

openssl rand -hex 16
来源：http://seq.ivvv.top

[R68] 计算文件校验值
来源：http://euy.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://taa.yj202588.top

[R69] 生成随机密码
来源：http://pfr.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://tfn.yuxming.cn

[R70] 时间戳与互转
来源：http://vlk.tanke756.top

date +%s;  date -d @1700000000
来源：http://njf.yonumen.top

[R71] 日期格式化
来源：http://uht.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://blm.gogol.net.cn

[R72] 等待端口就绪
来源：http://ndy.hcnkem.com

until nc -z localhost 3306; do sleep 1; done
来源：http://swx.zdbjq.cn

[R73] 分割大日志
来源：http://xew.sysykeji.top

split -l 1000 big.log part_
来源：http://lkz.52xcode.cn

[R74] 批量重命名
来源：http://ekt.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iey.zhoulong.xyz

[R75] 导出环境变量
来源：http://gnp.xingfuxueyuan.xyz

export PATH="$HOME/bin:$PATH"
来源：http://wcu.hongshengwenyu.top

[R76] 使用临时文件
来源：http://jlc.9152youxi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jmg.gogol.net.cn

[R77] 读取用户输入
来源：http://orr.xuanzx.com

read -rp "请输入: " ans
来源：http://toh.hnxiangtu.top

[R78] 交互式菜单
来源：http://fby.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dvd.gzhubu.top

[R79] 解析命令行选项
来源：http://sxt.hongshengwenyu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rpb.meibo888.top

[R80] 查看脚本执行耗时
来源：http://qeo.tarul.cn

time ./run.sh
来源：http://awa.aibaodan.cn

================================================================================
来源：http://osy.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://pqs.daxiang520.top

================================================================================
来源：http://xft.gogol.net.cn

[S01] C：Hello World
来源：http://xec.gzhubu.top

#include <stdio.h>
来源：http://pwz.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bjs.yuanzhike.top

[S02] C：变量与格式化输出
来源：http://tay.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://ahs.yongpay.top

[S03] C：读入整数
来源：http://bdg.xingfuxueyuan.xyz


<!-- 参考信息 -->