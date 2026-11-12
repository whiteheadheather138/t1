代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://rdf.hnxiangtu.top

JOIN users u ON u.id = o.user_id
来源：http://ckg.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://sgn.jinghuilouyu.cn

[Q42] 连接条件附加过滤
来源：http://vso.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u
来源：http://qgh.sufxvd.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bxu.yanxiufei.cn

[Q43] 标量子查询
来源：http://qdm.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://les.birdmap.top

[Q44] IN 子查询
来源：http://yiw.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iax.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://lxe.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hmm.hfpthk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://msl.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ymi.c1oappe.top

[Q47] 与平均值比较
来源：http://svn.jianghu66.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nyz.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://upc.tanke756.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://awd.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://uhv.tian-w.cn

[Q49] 更新单行
来源：http://bqz.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://otd.yanxiufei.cn

[Q50] 批量更新
来源：http://awk.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rpn.ydzc1.top

[Q51] 用子查询更新
来源：http://cub.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://noh.daxiang520.top

[Q52] 删除指定行
来源：http://eea.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://kpw.52xcode.cn

[Q53] 按条件删除
来源：http://hmi.yuxming.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iea.quarkkingdee.top

[Q54] 清空表
来源：http://gtl.wangshuangyany.cn

TRUNCATE TABLE logs;
来源：http://hjb.ywan-chungtsiang.top

[Q55] 排名（并列占位）
来源：http://run.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dcx.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://ihz.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hsd.aizwys.cn

[Q57] 行号
来源：http://tnz.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fbo.sweek.top

[Q58] 累计求和
来源：http://qia.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uwe.jianghu66.top

[Q59] 分组内累计
来源：http://jmj.pengpengdd.cyou

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jpc.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://nuj.sufxvd.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ihv.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qxp.hywenlv.cn

[Q61] 移动平均
来源：http://gwm.nanxinkj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://asw.yuxming.cn

[Q62] 分组占比
来源：http://bdz.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://udd.feifeiyinyue.top

[Q63] 开启事务
来源：http://wdn.ydzc1.top

START TRANSACTION;                -- 或 BEGIN
来源：http://coy.shanyushiyangtech.top

[Q64] 提交事务
来源：http://uwf.ctjpmb.com

COMMIT;
来源：http://bbp.chenlongwang.top

[Q65] 回滚事务
来源：http://tvi.bbcook.cn

ROLLBACK;
来源：http://xvv.daxiang520.top

[Q66] 行锁查询
来源：http://upp.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ohk.yueranfly.top

[Q67] 设置隔离级别
来源：http://eiw.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rjr.zhoulong.xyz

[Q68] 保存点
来源：http://afk.xuanzx.com

SAVEPOINT sp1;
来源：http://ame.hesvh.cn

ROLLBACK TO sp1;
来源：http://eqd.hywenlv.cn

[Q69] 查看执行计划
来源：http://frp.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vrp.meibo888.top

[Q70] 更新统计信息
来源：http://efl.fzhhl.top

ANALYZE TABLE users;
来源：http://mgv.yangfankeji.com

[Q71] 查看建表语句
来源：http://sjh.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cky.jinqigfzy.top

[Q72] 查看索引
来源：http://zia.xinyue.icu

SHOW INDEX FROM users;
来源：http://qpx.nanxuanxn.top

[Q73] 查看表状态
来源：http://fud.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bmh.pengpengdd.cyou

[Q74] 强制使用索引
来源：http://ltv.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xfe.ivvv.top

[Q75] 日期格式化
来源：http://hwk.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wvl.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ofg.wangshuangyany.cn

[Q76] 按天统计
来源：http://pez.yfazqb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jjn.hnxiangtu.top

[Q77] 时间加减
来源：http://mrm.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oyx.cashguo.top

[Q78] 当前时间
来源：http://qxj.jqgufenzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://top.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://nxs.aizwys.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://riz.guannengcc.top

[Q80] 字符串截取
来源：http://pmk.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lyb.mhx1999.top

[Q81] 字符串替换
来源：http://tyx.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tas.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://qzt.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ehu.bbcook.cn

[Q83] 大小写转换
来源：http://sal.0kj1m.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dom.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://xnf.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://rec.jqgufenzy.top

[Q85] 数值取整
来源：http://wjz.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://frw.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://gzf.yuanzhike.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eoi.hesvh.cn

[Q87] JSON 字段做条件
来源：http://uwo.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wrs.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://kzt.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://haq.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fli.pycfn.com

[Q89] 判断表是否存在
来源：http://yty.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xls.chenjidiqi.icu

[Q90] 生成序号列
来源：http://itw.birdmap.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gyn.kuanghao11.cn

================================================================================
来源：http://zip.vehdjk.com

R. Bash 专题
来源：http://mbv.snrcjt.cn

================================================================================
来源：http://uta.ehwqpu.com

[R01] shebang 与严格模式
来源：http://xpz.yongpay.top

#!/usr/bin/env bash
来源：http://xpm.birdmap.top

set -euo pipefail
来源：http://kty.zdqjudy.top

[R02] 变量赋值与使用
来源：http://ryt.aibaodan.cn

name="Tom"; echo "$name"
来源：http://mcq.zdqjudy.top

[R03] 只读变量
来源：http://sak.mhx1999.top

readonly PI=3.14
来源：http://nji.jinyuanbaomall.cn

[R04] 位置参数
来源：http://beg.uphjek.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nxd.0kj1m.cn

[R05] 参数默认值
来源：http://zps.hongshengwenyu.top

name="${1:-default}"
来源：http://ufe.fktsv.cn

[R06] 判断命令是否存在
来源：http://tgb.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nkh.yanxiufei.cn

[R07] if 判断文件
来源：http://yit.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ozy.ybcxt.top

[R08] 数值比较
来源：http://got.yfazqb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://yey.0kj1m.cn

[R09] 字符串比较
来源：http://cvi.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hvw.zdbjq.cn

[R10] 正则匹配
来源：http://uju.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kvz.fktsv.cn

[R11] case 多分支
来源：http://jvy.gotoacloud.top

case "$1" in
来源：http://zhg.cucudq.cn

start) echo "启动" ;;
来源：http://tox.hcnkem.com

stop)  echo "停止" ;;
来源：http://jhg.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://myi.pycfn.com

esac
来源：http://ago.hnqzz.top

[R12] for 遍历文件
来源：http://wfa.shzxlz.cn

for f in *.txt; do echo "$f"; done
来源：http://xex.daxiang520.top

[R13] for 计数循环
来源：http://uda.ivvv.top

for i in {1..10}; do echo "$i"; done
来源：http://qkg.svipenyu.cn

[R14] C 风格 for
来源：http://ibt.jinqigfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wei.chenlongwang.top

[R15] while 逐行读文件
来源：http://lsu.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sim.sjlbkw.cn

[R16] until 等待条件
来源：http://cyy.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cln.sufxvd.cn

[R17] 数组定义与取值
来源：http://tot.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://kkr.hammf.cn

[R18] 遍历数组
来源：http://bka.yonumen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cxb.aibaodan.cn

[R19] 数组长度
来源：http://knt.hongshengwenyu.top

echo "${#arr[@]}"
来源：http://ihk.hammf.cn

[R20] 关联数组（字典）
来源：http://eyw.cqqwz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ujx.nanxinkj.top

[R21] 字符串长度
来源：http://wun.bbcook.cn

echo "${#s}"
来源：http://mss.yanxiufei.cn

[R22] 截取子串
来源：http://ajh.jiagoushi.top

echo "${s:0:5}"
来源：http://ahy.ydjk.org.cn

[R23] 字符串替换
来源：http://nwy.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vbu.nanxinkj.top

[R24] 大小写转换
来源：http://lnb.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://qle.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://ubs.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jch.hywenlv.cn

[R26] 命令替换
来源：http://ccn.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://qaw.hnxiangtu.top

[R27] 算术展开
来源：http://adx.epnwcf.com

echo $((1 + 2 * 3))
来源：http://kdz.gaohongyu789.top

[R28] 浮点运算
来源：http://jgk.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://haj.cdnleiting.top

[R29] 定义函数
来源：http://xfn.jinyuanbaomall.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iao.yonumen.top

[R30] 函数返回状态码
来源：http://rdu.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://gad.chenlongwang.top

[R31] 局部变量
来源：http://fju.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://rxs.cdnleiting.top

[R32] 参数个数校验
来源：http://bcy.jinyuanbaomall.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gvf.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://uuw.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rau.52xcode.cn

[R34] 退出时清理
来源：http://lnv.feifeiyinyue.top

trap 'rm -f "$tmp"' EXIT
来源：http://fay.ydjk.org.cn

[R35] 后台执行并等待
来源：http://boa.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cgv.sufxvd.cn

[R36] 并发执行多个任务
来源：http://jzo.chenjidiqi.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nns.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://lna.hfpthk.cn

files=$(ls -1)
来源：http://cdm.yj202588.top

[R38] 管道串联
来源：http://kkn.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://qak.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://plp.iojbl.cn

cmd > out.log 2>&1
来源：http://nxx.52xcode.cn

[R40] 追加写日志
来源：http://cxn.zhixingplan.top

echo "log" >> out.log
来源：http://jko.yj202588.top

[R41] 丢弃输出
来源：http://zon.ydzc1.top

cmd >/dev/null 2>&1
来源：http://two.chenjidiqi.icu

[R42] 输入重定向
来源：http://oqi.zhoulong.xyz

wc -l < a.txt
来源：http://jzh.gaohongyu789.top

[R43] 按名字查找文件
来源：http://hem.fktsv.cn

find . -name "*.log" -type f
来源：http://xvo.yueranfly.top

[R44] 按修改时间查找
来源：http://zec.hammf.cn

find . -mtime -7 -type f
来源：http://xvw.yj202588.top

[R45] 批量删除
来源：http://alu.daria6918.cn

find . -name "*.tmp" -delete
来源：http://bel.aibaodan.cn

[R46] 递归替换文件内容
来源：http://pna.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pbo.tanke756.top

[R47] sed 单行替换
来源：http://jkz.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://neg.yj20258.top

[R48] awk 取指定列
来源：http://brr.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://eze.zhengqikj.top

[R49] awk 带条件
来源：http://vaz.yonumen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yyh.aibaodan.cn

[R50] awk 求和
来源：http://phg.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://ghp.zhongyouzk.top

[R51] 排序去重取前几
来源：http://dik.ybcxt.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pbt.ywan-chungtsiang.top

[R52] 统计行数
来源：http://rst.yj202588.top

wc -l a.txt
来源：http://dvh.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://hbk.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yfb.chenlongwang.top

[R54] 比较两个文件
来源：http://rwr.gotoacloud.top

diff a.txt b.txt
来源：http://ogn.hammf.cn

[R55] 压缩与解压
来源：http://ymi.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uac.gaohongyu789.top

[R56] 远程拷贝
来源：http://uvp.sjlbkw.cn

scp file user@host:/path/
来源：http://nes.guowangkeji.top

[R57] 远程执行命令
来源：http://ksi.yuanzhike.top

ssh user@host 'uptime'
来源：http://qzx.chenlongwang.top

[R58] 下载文件
来源：http://yra.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ldg.ctjpmb.com

[R59] 发 POST JSON
来源：http://aix.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://srm.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://xhc.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ext.ehwqpu.com

[R61] 磁盘占用
来源：http://yzm.zhixingplan.top

df -h;  du -sh *
来源：http://pin.daria6918.cn

[R62] 找最占空间的文件
来源：http://fph.vqdsnc.cn

du -ah . | sort -rh | head -10
来源：http://unt.sjlbkw.cn

[R63] 内存与进程
来源：http://znw.sweek.top

free -h;  ps aux | grep nginx
来源：http://jyo.haohaochexian.top

[R64] 结束进程
来源：http://unl.daria6918.cn

kill -9 $(pgrep -f app.py)
来源：http://gaq.jinqigfzy.top

[R65] 查看端口占用
来源：http://bio.meibo888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://krw.tianlin.xyz

[R66] 定时任务
来源：http://pks.chenzaomai.com

crontab -e;  crontab -l
来源：http://ikm.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://rsd.zhoulong.xyz

openssl rand -hex 16
来源：http://txm.iojbl.cn

[R68] 计算文件校验值
来源：http://fqp.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qln.xziqi.cn

[R69] 生成随机密码
来源：http://rrd.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://srg.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://vby.hammf.cn

date +%s;  date -d @1700000000
来源：http://gcs.cucudq.cn

[R71] 日期格式化
来源：http://taz.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://grx.cheryme.top

[R72] 等待端口就绪
来源：http://sab.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rty.hfpthk.cn

[R73] 分割大日志
来源：http://rzs.xziqi.cn

split -l 1000 big.log part_
来源：http://kkp.aizwys.cn

[R74] 批量重命名
来源：http://aam.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://odc.nwbrower.top

[R75] 导出环境变量
来源：http://qho.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://jex.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://fyi.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://veh.hnqzz.top

[R77] 读取用户输入
来源：http://ncs.chenzaomai.com

read -rp "请输入: " ans
来源：http://zba.316326.xyz

[R78] 交互式菜单
来源：http://rro.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qjx.daria6918.cn

[R79] 解析命令行选项
来源：http://kgv.yfazqb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bnp.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://ija.smart0.xyz

time ./run.sh
来源：http://yfv.feifeiyinyue.top

================================================================================
来源：http://yfz.xziqi.cn

S. C / C++ 专题
来源：http://edm.yfazqb.com

================================================================================
来源：http://gfo.daria6918.cn

[S01] C：Hello World
来源：http://ume.epnwcf.com

#include <stdio.h>
来源：http://udg.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://juc.wangshuangyany.cn

[S02] C：变量与格式化输出
来源：http://xep.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://pyn.hammf.cn

[S03] C：读入整数
来源：http://mqu.zdbjq.cn

int x; scanf("%d", &x);
来源：http://fyd.iojbl.cn

[S04] C：字符串复制
来源：http://qsd.shanyushiyangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://jco.hywenlv.cn

[S05] C：字符串长度
来源：http://jhi.zhaomingkeji.xyz

strlen(s)
来源：http://sqq.jinghuilouyu.cn

[S06] C：字符串比较
来源：http://msh.haohaochexian.top

strcmp(a, b) == 0
来源：http://woc.shanyushiyangtech.top

[S07] C：数组遍历求和
来源：http://vjk.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xdh.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://nyv.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ynm.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://vux.gotoacloud.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tmc.guannengcc.top

[S10] C：指针与解引用
来源：http://jkm.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://zyl.haohaochexian.top

[S11] C：逐行读文件
来源：http://ali.tian-w.cn


<!-- 参考信息 -->