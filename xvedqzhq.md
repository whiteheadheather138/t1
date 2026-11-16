代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dut.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://wan.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xti.ivvv.top

[Q41] 多表连接
来源：http://rmj.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://aju.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://ddu.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://tpv.sweek.top

[Q42] 连接条件附加过滤
来源：http://dbn.ydzc1.top

SELECT u.name, o.amount FROM users u
来源：http://rcf.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dro.cqqwz.cn

[Q43] 标量子查询
来源：http://vdu.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wfa.fehbvm.com

[Q44] IN 子查询
来源：http://sfl.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eso.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://skr.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cem.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://koz.ybcxt.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://olo.pycfn.com

[Q47] 与平均值比较
来源：http://ycw.zhoulong.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oat.sjlbkw.cn

[Q48] CTE 公用表表达式
来源：http://jvg.guowangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pxk.dianchejie.cn

SELECT * FROM t WHERE c > 5;
来源：http://idy.yj20258888.top

[Q49] 更新单行
来源：http://mmm.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dht.zhengqikj.top

[Q50] 批量更新
来源：http://gtl.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nef.shzxlz.cn

[Q51] 用子查询更新
来源：http://nkj.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xbl.andypj.xyz

[Q52] 删除指定行
来源：http://pmp.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://wld.kuanghao11.cn

[Q53] 按条件删除
来源：http://yqd.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dbb.cheryme.top

[Q54] 清空表
来源：http://bgg.zdbjq.cn

TRUNCATE TABLE logs;
来源：http://oss.52xcode.cn

[Q55] 排名（并列占位）
来源：http://qyg.havefunace.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jwf.zhengqikj.top

[Q56] 密集排名（并列不占位）
来源：http://xbi.yj20258.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dqu.shuidangran.top

[Q57] 行号
来源：http://suz.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://djy.xziqi.cn

[Q58] 累计求和
来源：http://hlt.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://atg.yuxming.cn

[Q59] 分组内累计
来源：http://gmy.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hsg.hnqzz.top

[Q60] 取上一行 / 下一行
来源：http://fxt.sjlbkw.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nlz.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iit.gogol.net.cn

[Q61] 移动平均
来源：http://oey.shanyushiyangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mxs.wangshuangyany.cn

[Q62] 分组占比
来源：http://fpc.chenlongwang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fcn.nanxuanxn.top

[Q63] 开启事务
来源：http://pav.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qml.aizwys.cn

[Q64] 提交事务
来源：http://zxa.hfpthk.cn

COMMIT;
来源：http://edy.ydjk.org.cn

[Q65] 回滚事务
来源：http://cqa.52xcode.cn

ROLLBACK;
来源：http://gof.daria6918.cn

[Q66] 行锁查询
来源：http://zai.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rcg.ydzc1.top

[Q67] 设置隔离级别
来源：http://ulh.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jxm.zhiwuduotai.top

[Q68] 保存点
来源：http://xgu.zhijiandao.cn

SAVEPOINT sp1;
来源：http://iqp.bbcook.cn

ROLLBACK TO sp1;
来源：http://wjo.ybcxt.top

[Q69] 查看执行计划
来源：http://hhg.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pkc.hfpthk.cn

[Q70] 更新统计信息
来源：http://ovw.0kj1m.cn

ANALYZE TABLE users;
来源：http://kkt.sweek.top

[Q71] 查看建表语句
来源：http://ffd.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jrv.smart0.xyz

[Q72] 查看索引
来源：http://prh.yongpay.top

SHOW INDEX FROM users;
来源：http://xkk.pengpengdd.cyou

[Q73] 查看表状态
来源：http://nyo.bjfxy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://shz.birdmap.top

[Q74] 强制使用索引
来源：http://hxt.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uvl.xingfuxueyuan.xyz

[Q75] 日期格式化
来源：http://gzf.sxryk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uyi.yangfankeji.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fyj.vehdjk.com

[Q76] 按天统计
来源：http://icv.yvedp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eop.zhengqikj.top

[Q77] 时间加减
来源：http://rnp.xziqi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jtt.gotoacloud.top

[Q78] 当前时间
来源：http://jav.ydzc1.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zgr.hcnkem.com

[Q79] 字符串拼接
来源：http://tea.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ylv.guowangkeji.top

[Q80] 字符串截取
来源：http://zxo.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aux.yvedp.cn

[Q81] 字符串替换
来源：http://rmx.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vce.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://uxp.xuanzx.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gjc.aizwys.cn

[Q83] 大小写转换
来源：http://idd.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gdl.jianghu66.top

[Q84] 去除首尾空格
来源：http://bqo.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://juz.chenlongwang.top

[Q85] 数值取整
来源：http://tbj.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ugw.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://gnn.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wdl.yj20258.top

[Q87] JSON 字段做条件
来源：http://frt.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tpy.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://pwp.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xri.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iav.ctjpmb.com

[Q89] 判断表是否存在
来源：http://nll.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uqt.yangfankeji.com

[Q90] 生成序号列
来源：http://knp.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wrj.fktsv.cn

================================================================================
来源：http://lke.ydjk.org.cn

R. Bash 专题
来源：http://zpp.sweek.top

================================================================================
来源：http://gxw.jqgfzy.top

[R01] shebang 与严格模式
来源：http://yud.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://vai.tianlin.xyz

set -euo pipefail
来源：http://lep.sxryk.cn

[R02] 变量赋值与使用
来源：http://jeg.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://qnt.havefunace.top

[R03] 只读变量
来源：http://mcp.jiagoushi.top

readonly PI=3.14
来源：http://aqv.shzxlz.cn

[R04] 位置参数
来源：http://xyy.smart0.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lsr.sysykeji.top

[R05] 参数默认值
来源：http://mem.xuetiantiany.cn

name="${1:-default}"
来源：http://tao.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://hsr.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://obx.hcnkem.com

[R07] if 判断文件
来源：http://dfs.epnwcf.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fpe.yangfankeji.com

[R08] 数值比较
来源：http://doh.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://thd.gaohongyu789.top

[R09] 字符串比较
来源：http://zge.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gwi.tanke756.top

[R10] 正则匹配
来源：http://dew.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pgt.jinghuilouyu.cn

[R11] case 多分支
来源：http://sey.yanxiufei.cn

case "$1" in
来源：http://pgq.zhiwuduotai.top

start) echo "启动" ;;
来源：http://yqz.hesvh.cn

stop)  echo "停止" ;;
来源：http://vwl.yanxiufei.cn

*)     echo "未知命令" ;;
来源：http://tki.cqqwz.cn

esac
来源：http://qdt.tian-w.cn

[R12] for 遍历文件
来源：http://cbo.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://jxv.aibaodan.cn

[R13] for 计数循环
来源：http://ivr.yonumen.top

for i in {1..10}; do echo "$i"; done
来源：http://abo.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://rhr.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bop.svipenyu.cn

[R15] while 逐行读文件
来源：http://hte.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rjo.hywenlv.cn

[R16] until 等待条件
来源：http://rfo.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hex.chenjidiqi.icu

[R17] 数组定义与取值
来源：http://eqn.xuanzx.com

arr=(a b c); echo "${arr[0]}"
来源：http://ttj.daria6918.cn

[R18] 遍历数组
来源：http://wiv.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qgv.dianchejie.cn

[R19] 数组长度
来源：http://uuv.0kj1m.cn

echo "${#arr[@]}"
来源：http://fzb.bbcook.cn

[R20] 关联数组（字典）
来源：http://dau.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pdf.chenlongwang.top

[R21] 字符串长度
来源：http://wbn.jinqigfzy.top

echo "${#s}"
来源：http://oii.feifeiyinyue.top

[R22] 截取子串
来源：http://xev.mhx1999.top

echo "${s:0:5}"
来源：http://rxh.cqqwz.cn

[R23] 字符串替换
来源：http://ttu.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rmb.haohaochexian.top

[R24] 大小写转换
来源：http://bcu.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://tdz.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://ojm.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fyu.sjlbkw.cn

[R26] 命令替换
来源：http://bol.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://yuo.fehbvm.com

[R27] 算术展开
来源：http://imc.jinqigfzy.top

echo $((1 + 2 * 3))
来源：http://fai.ivvv.top

[R28] 浮点运算
来源：http://ebz.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://efb.yfazqb.com

[R29] 定义函数
来源：http://njz.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ukr.chenlongwang.top

[R30] 函数返回状态码
来源：http://ufn.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://bsr.dianchejie.cn

[R31] 局部变量
来源：http://fgm.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://mot.yanxiufei.cn

[R32] 参数个数校验
来源：http://ftd.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nbk.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://zed.ehwqpu.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vfr.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://biq.52xcode.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eqr.tanke756.top

[R35] 后台执行并等待
来源：http://mfr.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://olc.fktsv.cn

[R36] 并发执行多个任务
来源：http://sgh.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mua.0kj1m.cn

[R37] 把输出赋给变量
来源：http://biq.ywan-chungtsiang.top

files=$(ls -1)
来源：http://zdm.yonumen.top

[R38] 管道串联
来源：http://hqc.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://qkv.ydzc1.top

[R39] 重定向标准输出与错误
来源：http://mzi.tian-w.cn

cmd > out.log 2>&1
来源：http://vfk.dianchejie.cn

[R40] 追加写日志
来源：http://hjd.shangyingyoupin.top

echo "log" >> out.log
来源：http://vel.sjlbkw.cn

[R41] 丢弃输出
来源：http://igh.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://jnb.yuanzhike.top

[R42] 输入重定向
来源：http://ngt.daria6918.cn

wc -l < a.txt
来源：http://tfr.hysaishi.cn

[R43] 按名字查找文件
来源：http://wxv.yj20258888.top

find . -name "*.log" -type f
来源：http://nhn.yongpay.top

[R44] 按修改时间查找
来源：http://ayd.cheryme.top

find . -mtime -7 -type f
来源：http://srd.guowangkeji.top

[R45] 批量删除
来源：http://pxt.ydjk.org.cn

find . -name "*.tmp" -delete
来源：http://spp.yueranfly.top

[R46] 递归替换文件内容
来源：http://saf.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vpc.hnqzz.top

[R47] sed 单行替换
来源：http://upi.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://kjz.kuanghao11.cn

[R48] awk 取指定列
来源：http://ilo.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://jvt.jyoumei.cn

[R49] awk 带条件
来源：http://uzj.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gdg.cashguo.top

[R50] awk 求和
来源：http://knf.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://uzx.birdmap.top

[R51] 排序去重取前几
来源：http://ifs.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tit.yfazqb.com

[R52] 统计行数
来源：http://eqq.xingfuxueyuan.xyz

wc -l a.txt
来源：http://kpe.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://eia.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sen.c1oappe.top

[R54] 比较两个文件
来源：http://gbg.vqdsnc.cn

diff a.txt b.txt
来源：http://eco.aibaodan.cn

[R55] 压缩与解压
来源：http://scl.fanxiaobao.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://crt.c1oappe.top

[R56] 远程拷贝
来源：http://now.wangdashe.top

scp file user@host:/path/
来源：http://rpy.jinqigfzy.top

[R57] 远程执行命令
来源：http://scb.nanxinkj.top

ssh user@host 'uptime'
来源：http://mab.316326.xyz

[R58] 下载文件
来源：http://fjz.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wii.fengsongda.top

[R59] 发 POST JSON
来源：http://mdy.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://str.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://pvc.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gyk.yonumen.top

[R61] 磁盘占用
来源：http://jff.hongshengwenyu.top

df -h;  du -sh *
来源：http://ons.cashguo.top

[R62] 找最占空间的文件
来源：http://zuw.zhiwuduotai.top

du -ah . | sort -rh | head -10
来源：http://ehc.zdqjudy.top

[R63] 内存与进程
来源：http://cpb.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://swf.vqdsnc.cn

[R64] 结束进程
来源：http://bji.jinghuilouyu.cn

kill -9 $(pgrep -f app.py)
来源：http://swr.vqdsnc.cn

[R65] 查看端口占用
来源：http://otx.zhixingplan.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sjv.yueranfly.top

[R66] 定时任务
来源：http://vcr.yongpay.top

crontab -e;  crontab -l
来源：http://ezk.hysaishi.cn

[R67] 生成随机十六进制串
来源：http://rqo.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://kcs.ybcxt.top

[R68] 计算文件校验值
来源：http://ojp.tian-w.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rzm.uphjek.com

[R69] 生成随机密码
来源：http://zxy.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://ugn.dashuyun.cn

[R70] 时间戳与互转
来源：http://cxu.316326.xyz

date +%s;  date -d @1700000000
来源：http://fyz.zhiwuduotai.top

[R71] 日期格式化
来源：http://vdc.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zuk.daxiang520.top

[R72] 等待端口就绪
来源：http://bjl.hywenlv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ggi.svipenyu.cn

[R73] 分割大日志
来源：http://twj.jianghu66.top

split -l 1000 big.log part_
来源：http://nmf.bjfxy.top

[R74] 批量重命名
来源：http://nlr.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ffc.aibaodan.cn

[R75] 导出环境变量
来源：http://qmg.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://olh.0kj1m.cn

[R76] 使用临时文件
来源：http://jna.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jcv.xuetiantiany.cn

[R77] 读取用户输入
来源：http://ekk.bjfxy.top

read -rp "请输入: " ans
来源：http://zoz.xinyue.icu

[R78] 交互式菜单
来源：http://pwd.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ipx.fktsv.cn

[R79] 解析命令行选项
来源：http://cvh.smart0.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jmu.yj202588.top

[R80] 查看脚本执行耗时
来源：http://qgh.hfpthk.cn

time ./run.sh
来源：http://rsq.sjlbkw.cn

================================================================================
来源：http://ozu.fehbvm.com

S. C / C++ 专题
来源：http://fhh.yvedp.cn

================================================================================
来源：http://ygm.9152youxi.cn

[S01] C：Hello World
来源：http://zrj.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://jgi.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mal.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://tkj.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://srq.shuidangran.top

[S03] C：读入整数
来源：http://eww.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://iie.jiagoushi.top

[S04] C：字符串复制
来源：http://lbm.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://krr.yj20258888.top

[S05] C：字符串长度
来源：http://gxy.xingfuxueyuan.xyz

strlen(s)
来源：http://dmb.kuanghao11.cn

[S06] C：字符串比较
来源：http://cbd.ydzc1.top

strcmp(a, b) == 0
来源：http://ont.mhx1999.top

[S07] C：数组遍历求和
来源：http://pac.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://thc.jqgfzy.top

[S08] C：动态内存分配与释放
来源：http://jwq.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wmg.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://ypv.xinyue.icu


<!-- 参考信息 -->