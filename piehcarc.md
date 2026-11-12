代发 wailian999

[Q36] 左连接
来源：http://mog.zhongyouzk.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xge.pengpengdd.cyou

[Q37] 右连接
来源：http://jwk.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lnq.yvedp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lap.jqgufenzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yin.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://uhc.316326.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://xtk.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ddb.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zrx.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lmz.zdbjq.cn

[Q41] 多表连接
来源：http://uon.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ety.9152youxi.cn

JOIN users u ON u.id = o.user_id
来源：http://nea.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://tst.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://cgw.cucudq.cn

SELECT u.name, o.amount FROM users u
来源：http://jnv.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://juz.zhongyouzk.top

[Q43] 标量子查询
来源：http://izn.0kj1m.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://okr.shzxlz.cn

[Q44] IN 子查询
来源：http://gde.cdnleiting.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vks.sweek.top

[Q45] EXISTS 判断存在
来源：http://hbc.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hrh.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bsd.fehbvm.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rut.yfazqb.com

[Q47] 与平均值比较
来源：http://vdt.yvedp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://liu.sufxvd.cn

[Q48] CTE 公用表表达式
来源：http://peq.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ccr.chenlongwang.top

SELECT * FROM t WHERE c > 5;
来源：http://xyr.jqgfzy.top

[Q49] 更新单行
来源：http://mbm.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jzk.nwbrower.top

[Q50] 批量更新
来源：http://wmv.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tqw.yonumen.top

[Q51] 用子查询更新
来源：http://hsq.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oyr.jiagoushi.top

[Q52] 删除指定行
来源：http://jiw.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://tsu.aibaodan.cn

[Q53] 按条件删除
来源：http://atl.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://auv.ivvv.top

[Q54] 清空表
来源：http://lrw.xylfe.cn

TRUNCATE TABLE logs;
来源：http://ofr.wangdashe.top

[Q55] 排名（并列占位）
来源：http://qpz.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vvr.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://gjn.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xqq.hcnkem.com

[Q57] 行号
来源：http://kky.52xcode.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xpz.ehwqpu.com

[Q58] 累计求和
来源：http://klc.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aax.nanxuanxn.top

[Q59] 分组内累计
来源：http://gek.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tgp.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://aha.tianlin.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://inm.ydjk.org.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://scy.tanke756.top

[Q61] 移动平均
来源：http://vxo.yuanzhike.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xoj.jiagoushi.top

[Q62] 分组占比
来源：http://ile.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wjb.shangyingyoupin.top

[Q63] 开启事务
来源：http://iwb.vehdjk.com

START TRANSACTION;                -- 或 BEGIN
来源：http://tuc.yueranfly.top

[Q64] 提交事务
来源：http://htf.bjfxy.top

COMMIT;
来源：http://kmj.aizwys.cn

[Q65] 回滚事务
来源：http://tee.tian-w.cn

ROLLBACK;
来源：http://cfo.jqgufenzy.top

[Q66] 行锁查询
来源：http://gur.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://row.gzhubu.top

[Q67] 设置隔离级别
来源：http://xsq.dianchejie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://emq.svipenyu.cn

[Q68] 保存点
来源：http://nbu.nanxinkj.top

SAVEPOINT sp1;
来源：http://qlg.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://agd.pengpengdd.cyou

[Q69] 查看执行计划
来源：http://iwc.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gcy.tianlin.xyz

[Q70] 更新统计信息
来源：http://ziq.aibaodan.cn

ANALYZE TABLE users;
来源：http://xzp.mhx1999.top

[Q71] 查看建表语句
来源：http://ffd.iojbl.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xmj.hfpthk.cn

[Q72] 查看索引
来源：http://xuz.vehdjk.com

SHOW INDEX FROM users;
来源：http://ypj.zhijiandao.cn

[Q73] 查看表状态
来源：http://jvz.tanke756.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ewm.zdqjudy.top

[Q74] 强制使用索引
来源：http://enl.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ojz.yj20258.top

[Q75] 日期格式化
来源：http://bvn.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bqo.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bto.9152youxi.cn

[Q76] 按天统计
来源：http://hlh.hesvh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ccq.vehdjk.com

[Q77] 时间加减
来源：http://wej.gogol.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wzh.ybcxt.top

[Q78] 当前时间
来源：http://lyj.gaohongyu789.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ldb.birdmap.top

[Q79] 字符串拼接
来源：http://tcq.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ibm.chenjidiqi.icu

[Q80] 字符串截取
来源：http://mcp.zdbjq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qye.guowangkeji.top

[Q81] 字符串替换
来源：http://jpr.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://net.zhixingplan.top

[Q82] 字符长度与字节长度
来源：http://ejr.bbcook.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://njg.jlsjyb.cn

[Q83] 大小写转换
来源：http://ntx.chenjidiqi.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://upg.andypj.xyz

[Q84] 去除首尾空格
来源：http://glb.zhaomingkeji.xyz

SELECT TRIM(name) FROM users;
来源：http://juu.hongshengwenyu.top

[Q85] 数值取整
来源：http://unv.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vfq.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://cgl.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zin.sxryk.cn

[Q87] JSON 字段做条件
来源：http://wwp.hfpthk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://exe.52xcode.cn

[Q88] 行转列（条件聚合）
来源：http://uwg.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lub.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zel.bbcook.cn

[Q89] 判断表是否存在
来源：http://wph.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hqh.gotoacloud.top

[Q90] 生成序号列
来源：http://uzt.tarul.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hmh.xuanzx.com

================================================================================
来源：http://wcj.meibo888.top

R. Bash 专题
来源：http://may.nanxuanxn.top

================================================================================
来源：http://psw.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://dqr.hesvh.cn

#!/usr/bin/env bash
来源：http://guc.pengpengdd.cyou

set -euo pipefail
来源：http://xgl.ivvv.top

[R02] 变量赋值与使用
来源：http://zav.kuanghao11.cn

name="Tom"; echo "$name"
来源：http://gkz.bbcook.cn

[R03] 只读变量
来源：http://cgv.fktsv.cn

readonly PI=3.14
来源：http://wnb.havefunace.top

[R04] 位置参数
来源：http://eoy.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nrk.bbcook.cn

[R05] 参数默认值
来源：http://hmh.fengsongda.top

name="${1:-default}"
来源：http://ego.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://ciw.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dju.wangshuangyany.cn

[R07] if 判断文件
来源：http://jiy.yonumen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zqz.chenzaomai.com

[R08] 数值比较
来源：http://jvz.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zbt.fehbvm.com

[R09] 字符串比较
来源：http://jst.epnwcf.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uqj.0kj1m.cn

[R10] 正则匹配
来源：http://xfr.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rpe.xylfe.cn

[R11] case 多分支
来源：http://itm.tanke756.top

case "$1" in
来源：http://hib.vqdsnc.cn

start) echo "启动" ;;
来源：http://atn.hammf.cn

stop)  echo "停止" ;;
来源：http://hbj.havefunace.top

*)     echo "未知命令" ;;
来源：http://rrc.vehdjk.com

esac
来源：http://pgj.yonumen.top

[R12] for 遍历文件
来源：http://xqu.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://ikv.dashuyun.cn

[R13] for 计数循环
来源：http://bvr.hesvh.cn

for i in {1..10}; do echo "$i"; done
来源：http://psa.ivvv.top

[R14] C 风格 for
来源：http://geq.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iyj.wangdashe.top

[R15] while 逐行读文件
来源：http://fqv.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jvi.jiagoushi.top

[R16] until 等待条件
来源：http://lpf.smart0.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://clg.0kj1m.cn

[R17] 数组定义与取值
来源：http://ruy.feifeiyinyue.top

arr=(a b c); echo "${arr[0]}"
来源：http://ctf.zdbjq.cn

[R18] 遍历数组
来源：http://mch.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://loe.yuxming.cn

[R19] 数组长度
来源：http://niu.vehdjk.com

echo "${#arr[@]}"
来源：http://abb.yangfankeji.com

[R20] 关联数组（字典）
来源：http://xpr.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dmx.yfazqb.com

[R21] 字符串长度
来源：http://ten.sxryk.cn

echo "${#s}"
来源：http://lnw.sxryk.cn

[R22] 截取子串
来源：http://dvd.hysaishi.cn

echo "${s:0:5}"
来源：http://pqt.mhx1999.top

[R23] 字符串替换
来源：http://ygl.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qki.chenlongwang.top

[R24] 大小写转换
来源：http://oqe.ywan-chungtsiang.top

echo "${s^^}"; echo "${s,,}"
来源：http://pbg.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://tpb.yongpay.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://msb.daria6918.cn

[R26] 命令替换
来源：http://heu.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://ute.hammf.cn

[R27] 算术展开
来源：http://nwh.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://usg.zhiwuduotai.top

[R28] 浮点运算
来源：http://tbe.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://cog.vehdjk.com

[R29] 定义函数
来源：http://fad.jinyuanbaomall.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://caq.jqgufenzy.top

[R30] 函数返回状态码
来源：http://nor.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://bzp.ydzc1.top

[R31] 局部变量
来源：http://euw.haohaochexian.top

f() { local x=1; echo "$x"; }
来源：http://iei.zycfv.cn

[R32] 参数个数校验
来源：http://afa.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hyf.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://ort.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bsq.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://fpx.jinqigfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://yzd.shzxlz.cn

[R35] 后台执行并等待
来源：http://uvk.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://uza.zhijiandao.cn

[R36] 并发执行多个任务
来源：http://hku.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mkw.tian-w.cn

[R37] 把输出赋给变量
来源：http://jqz.guowangkeji.top

files=$(ls -1)
来源：http://www.jiagoushi.top

[R38] 管道串联
来源：http://lsl.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://hgt.9152youxi.cn

[R39] 重定向标准输出与错误
来源：http://srs.andypj.xyz

cmd > out.log 2>&1
来源：http://hlu.ppjwa.cn

[R40] 追加写日志
来源：http://aqi.hysaishi.cn

echo "log" >> out.log
来源：http://dkg.zdqjudy.top

[R41] 丢弃输出
来源：http://www.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://kox.chenzaomai.com

[R42] 输入重定向
来源：http://bvu.jinyuanbaomall.cn

wc -l < a.txt
来源：http://uky.zhixingplan.top

[R43] 按名字查找文件
来源：http://zyx.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://iox.iojbl.cn

[R44] 按修改时间查找
来源：http://aad.epnwcf.com

find . -mtime -7 -type f
来源：http://ius.9152youxi.cn

[R45] 批量删除
来源：http://pfj.316326.xyz

find . -name "*.tmp" -delete
来源：http://pif.zhijiandao.cn

[R46] 递归替换文件内容
来源：http://tth.ctjpmb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vmf.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://qgx.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gmb.zhongyouzk.top

[R48] awk 取指定列
来源：http://bpn.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://ahg.chenlongwang.top

[R49] awk 带条件
来源：http://sit.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bne.zdqjudy.top

[R50] awk 求和
来源：http://tyw.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://ymu.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://tgk.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://qgh.sxryk.cn

[R52] 统计行数
来源：http://nat.nanxuanxn.top

wc -l a.txt
来源：http://wku.yonumen.top

[R53] 查看文件头与实时尾
来源：http://nbg.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://smm.cheryme.top

[R54] 比较两个文件
来源：http://wuo.nanxinkj.top

diff a.txt b.txt
来源：http://gzd.nwbrower.top

[R55] 压缩与解压
来源：http://vdi.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wbw.zhixingplan.top

[R56] 远程拷贝
来源：http://akz.dianchejie.cn

scp file user@host:/path/
来源：http://yjv.ydjk.org.cn

[R57] 远程执行命令
来源：http://rzf.yvedp.cn

ssh user@host 'uptime'
来源：http://qhu.zhijiandao.cn

[R58] 下载文件
来源：http://hum.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://etk.jqgfzy.top

[R59] 发 POST JSON
来源：http://yzv.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zsf.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://cho.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fkc.zhoulong.xyz

[R61] 磁盘占用
来源：http://ujq.ybcxt.top

df -h;  du -sh *
来源：http://vcp.gaohongyu789.top

[R62] 找最占空间的文件
来源：http://tsn.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://ptn.tian-w.cn

[R63] 内存与进程
来源：http://irj.nanxuanxn.top

free -h;  ps aux | grep nginx
来源：http://gsr.zhixingplan.top

[R64] 结束进程
来源：http://uzw.meibo888.top

kill -9 $(pgrep -f app.py)
来源：http://xkp.cheryme.top

[R65] 查看端口占用
来源：http://ggt.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gyg.hfpthk.cn

[R66] 定时任务
来源：http://xdp.tarul.cn

crontab -e;  crontab -l
来源：http://gon.yvedp.cn

[R67] 生成随机十六进制串
来源：http://ggu.ehwqpu.com

openssl rand -hex 16
来源：http://hve.sxryk.cn

[R68] 计算文件校验值
来源：http://edl.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://suz.iojbl.cn

[R69] 生成随机密码
来源：http://mes.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://lap.yj20258.top

[R70] 时间戳与互转
来源：http://jgh.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://pmd.shuidangran.top

[R71] 日期格式化
来源：http://yfk.sysykeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qaq.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://qgs.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wup.zdqjudy.top

[R73] 分割大日志
来源：http://nnr.cucudq.cn

split -l 1000 big.log part_
来源：http://vim.pycfn.com

[R74] 批量重命名
来源：http://fig.meibo888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://axw.0kj1m.cn

[R75] 导出环境变量
来源：http://ypa.hywenlv.cn

export PATH="$HOME/bin:$PATH"
来源：http://eno.fktsv.cn

[R76] 使用临时文件
来源：http://wxx.smart0.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ckx.0kj1m.cn

[R77] 读取用户输入
来源：http://zpy.nanxinkj.top

read -rp "请输入: " ans
来源：http://tvc.9152youxi.cn

[R78] 交互式菜单
来源：http://pav.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qmv.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://bmz.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://txb.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://ebl.redwolf501.top

time ./run.sh
来源：http://mhu.snrcjt.cn

================================================================================
来源：http://dtg.yj20258.top

S. C / C++ 专题
来源：http://bxf.jqgfzy.top

================================================================================
来源：http://lug.zdbjq.cn

[S01] C：Hello World
来源：http://ido.tianlin.xyz

#include <stdio.h>
来源：http://lvs.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jyc.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://dga.guannengcc.top

int a = 10; printf("%d\n", a);
来源：http://rqh.feifeiyinyue.top

[S03] C：读入整数
来源：http://ieg.guannengcc.top

int x; scanf("%d", &x);
来源：http://yfg.zycfv.cn

[S04] C：字符串复制
来源：http://kwe.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://ilm.chenlongwang.top

[S05] C：字符串长度
来源：http://fav.jianghu66.top


<!-- 参考信息 -->