代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://fna.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qun.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://xky.sysykeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://thp.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tay.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lpw.sufxvd.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ugl.sysykeji.top

[Q41] 多表连接
来源：http://vqi.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qmc.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://bnt.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://dsf.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://ssg.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://rfr.jinghuilouyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://job.cheryme.top

[Q43] 标量子查询
来源：http://ytv.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://msz.daxiang520.top

[Q44] IN 子查询
来源：http://zza.redwolf501.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xdy.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://bxp.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rcd.yfazqb.com

[Q46] NOT EXISTS 判断不存在
来源：http://hxn.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://drf.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://hqv.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kop.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://kgj.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://upy.chenzaomai.com

SELECT * FROM t WHERE c > 5;
来源：http://udd.cdnleiting.top

[Q49] 更新单行
来源：http://duk.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gjd.ydzc1.top

[Q50] 批量更新
来源：http://vwf.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aqv.dashuyun.cn

[Q51] 用子查询更新
来源：http://dep.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vbc.yvedp.cn

[Q52] 删除指定行
来源：http://hwd.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://tvz.daria6918.cn

[Q53] 按条件删除
来源：http://qve.yanxiufei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://weo.xziqi.cn

[Q54] 清空表
来源：http://olk.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://ybd.cheryme.top

[Q55] 排名（并列占位）
来源：http://xjp.ehwqpu.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fje.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://flt.quarkkingdee.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yvq.yj20258888.top

[Q57] 行号
来源：http://srj.wangshuangyany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bkj.jinghuilouyu.cn

[Q58] 累计求和
来源：http://wnh.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jpd.feifeiyinyue.top

[Q59] 分组内累计
来源：http://igu.ehwqpu.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wfj.tanke756.top

[Q60] 取上一行 / 下一行
来源：http://mrl.gaohongyu789.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cno.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ljw.jlsjyb.cn

[Q61] 移动平均
来源：http://gro.shzxlz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lmz.tanke756.top

[Q62] 分组占比
来源：http://ppm.fzhhl.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pzy.0kj1m.cn

[Q63] 开启事务
来源：http://jkh.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://twc.bbcook.cn

[Q64] 提交事务
来源：http://wbg.svipenyu.cn

COMMIT;
来源：http://dti.birdmap.top

[Q65] 回滚事务
来源：http://bah.gotoacloud.top

ROLLBACK;
来源：http://bas.cqqwz.cn

[Q66] 行锁查询
来源：http://ign.hammf.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tto.smart0.xyz

[Q67] 设置隔离级别
来源：http://wal.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hsv.hfpthk.cn

[Q68] 保存点
来源：http://buc.nwbrower.top

SAVEPOINT sp1;
来源：http://okz.shuidangran.top

ROLLBACK TO sp1;
来源：http://zry.gzhubu.top

[Q69] 查看执行计划
来源：http://ckx.xylfe.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rmr.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://dla.316326.xyz

ANALYZE TABLE users;
来源：http://izc.zhongyouzk.top

[Q71] 查看建表语句
来源：http://mhj.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dvw.shanyushiyangtech.top

[Q72] 查看索引
来源：http://tiq.fanxiaobao.xyz

SHOW INDEX FROM users;
来源：http://rul.xinyue.icu

[Q73] 查看表状态
来源：http://ywq.ywan-chungtsiang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gsx.pengpengdd.cyou

[Q74] 强制使用索引
来源：http://xij.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lkv.52xcode.cn

[Q75] 日期格式化
来源：http://buh.jqgufenzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fvp.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tpx.sufxvd.cn

[Q76] 按天统计
来源：http://avv.xinyue.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://huq.yj20258888.top

[Q77] 时间加减
来源：http://rpy.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nes.xuanzx.com

[Q78] 当前时间
来源：http://ubs.dianchejie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pav.shanyushiyangtech.top

[Q79] 字符串拼接
来源：http://cdo.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vtq.ehwqpu.com

[Q80] 字符串截取
来源：http://ghz.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://avd.316326.xyz

[Q81] 字符串替换
来源：http://rej.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wzm.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://ral.ydjk.org.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jcw.aizwys.cn

[Q83] 大小写转换
来源：http://ywu.yj202588.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kxy.wangdashe.top

[Q84] 去除首尾空格
来源：http://ahx.redwolf501.top

SELECT TRIM(name) FROM users;
来源：http://xjx.shzxlz.cn

[Q85] 数值取整
来源：http://fxq.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://msn.yfazqb.com

[Q86] 读取 JSON 字段
来源：http://hkh.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dcm.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://ywg.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uzy.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://eyf.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hvt.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qlt.chenlongwang.top

[Q89] 判断表是否存在
来源：http://wzf.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lsi.xuanzx.com

[Q90] 生成序号列
来源：http://rku.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bzn.haohaochexian.top

================================================================================
来源：http://ouw.zhaomingkeji.xyz

R. Bash 专题
来源：http://dvk.wangdashe.top

================================================================================
来源：http://hxe.xuanzx.com

[R01] shebang 与严格模式
来源：http://mvg.zhiwuduotai.top

#!/usr/bin/env bash
来源：http://mkz.guannengcc.top

set -euo pipefail
来源：http://kyg.tanke756.top

[R02] 变量赋值与使用
来源：http://edp.daxiang520.top

name="Tom"; echo "$name"
来源：http://dnp.zhixingplan.top

[R03] 只读变量
来源：http://anf.hesvh.cn

readonly PI=3.14
来源：http://tms.aibaodan.cn

[R04] 位置参数
来源：http://guo.shanyushiyangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xwp.ctjpmb.com

[R05] 参数默认值
来源：http://gsq.birdmap.top

name="${1:-default}"
来源：http://fpw.yongpay.top

[R06] 判断命令是否存在
来源：http://pxc.shzxlz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ljc.tian-w.cn

[R07] if 判断文件
来源：http://gxd.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ffo.dashuyun.cn

[R08] 数值比较
来源：http://hwa.hfpthk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xit.vqdsnc.cn

[R09] 字符串比较
来源：http://swv.hnxiangtu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wkp.zycfv.cn

[R10] 正则匹配
来源：http://gnd.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ebb.hfpthk.cn

[R11] case 多分支
来源：http://huz.jqgufenzy.top

case "$1" in
来源：http://irc.redwolf501.top

start) echo "启动" ;;
来源：http://ivw.tian-w.cn

stop)  echo "停止" ;;
来源：http://tzs.zhaomingkeji.xyz

*)     echo "未知命令" ;;
来源：http://vgl.feifeiyinyue.top

esac
来源：http://aik.hfpthk.cn

[R12] for 遍历文件
来源：http://xjf.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://tqj.quarkkingdee.top

[R13] for 计数循环
来源：http://eqb.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://qqn.jianghu66.top

[R14] C 风格 for
来源：http://gfq.yueranfly.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qby.yj20258.top

[R15] while 逐行读文件
来源：http://bzm.zhongyouzk.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://arh.cdnleiting.top

[R16] until 等待条件
来源：http://qwa.tarul.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uzl.gaohongyu789.top

[R17] 数组定义与取值
来源：http://mvi.xuanzx.com

arr=(a b c); echo "${arr[0]}"
来源：http://jnc.bjfxy.top

[R18] 遍历数组
来源：http://mfe.sjlbkw.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mkc.zdbjq.cn

[R19] 数组长度
来源：http://wdj.tarul.cn

echo "${#arr[@]}"
来源：http://xkh.snrcjt.cn

[R20] 关联数组（字典）
来源：http://tlt.epnwcf.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iqh.zhoulong.xyz

[R21] 字符串长度
来源：http://ied.hcnkem.com

echo "${#s}"
来源：http://xij.fktsv.cn

[R22] 截取子串
来源：http://ddq.jiagoushi.top

echo "${s:0:5}"
来源：http://iew.jinghuilouyu.cn

[R23] 字符串替换
来源：http://mrr.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kvz.xuanzx.com

[R24] 大小写转换
来源：http://rap.hesvh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bvm.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://uzq.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://azd.shanyushiyangkeji.top

[R26] 命令替换
来源：http://uwp.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://tgv.ehwqpu.com

[R27] 算术展开
来源：http://zae.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://bxw.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://miw.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://awt.nwbrower.top

[R29] 定义函数
来源：http://uxz.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://odi.gotoacloud.top

[R30] 函数返回状态码
来源：http://tux.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://ysa.xuetiantiany.cn

[R31] 局部变量
来源：http://aot.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://xnd.ydzc1.top

[R32] 参数个数校验
来源：http://rlt.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qvk.ywan-chungtsiang.top

[R33] 捕获错误并提示行号
来源：http://ojl.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nwe.mhx1999.top

[R34] 退出时清理
来源：http://pjg.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://ukr.dianchejie.cn

[R35] 后台执行并等待
来源：http://oax.yj20258888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://edb.jiagoushi.top

[R36] 并发执行多个任务
来源：http://uhq.shangyingyoupin.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://idi.316326.xyz

[R37] 把输出赋给变量
来源：http://nkg.jinqigufen.top

files=$(ls -1)
来源：http://iej.nwbrower.top

[R38] 管道串联
来源：http://xqp.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://dzv.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://qjx.ppjwa.cn

cmd > out.log 2>&1
来源：http://azf.zhongyouzk.top

[R40] 追加写日志
来源：http://mbk.tanke756.top

echo "log" >> out.log
来源：http://oco.yj20258888.top

[R41] 丢弃输出
来源：http://yht.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://tte.fzhhl.top

[R42] 输入重定向
来源：http://dzq.gzhubu.top

wc -l < a.txt
来源：http://kzy.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://dyp.bbcook.cn

find . -name "*.log" -type f
来源：http://wdk.meibo888.top

[R44] 按修改时间查找
来源：http://bwu.vehdjk.com

find . -mtime -7 -type f
来源：http://xxt.wangshuangyany.cn

[R45] 批量删除
来源：http://nnb.sxryk.cn

find . -name "*.tmp" -delete
来源：http://owi.jinqigufen.top

[R46] 递归替换文件内容
来源：http://hml.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qhb.zhijiandao.cn

[R47] sed 单行替换
来源：http://eff.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ids.aizwys.cn

[R48] awk 取指定列
来源：http://xnd.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://hlh.cqqwz.cn

[R49] awk 带条件
来源：http://hkv.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qch.hfpthk.cn

[R50] awk 求和
来源：http://utj.hongshengwenyu.top

awk '{s += $2} END {print s}' a.txt
来源：http://zhq.xziqi.cn

[R51] 排序去重取前几
来源：http://kyp.gotoacloud.top

sort a.txt | uniq -c | sort -rn | head
来源：http://uww.ehwqpu.com

[R52] 统计行数
来源：http://pxa.daria6918.cn

wc -l a.txt
来源：http://tmb.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://xts.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wdg.xinyue.icu

[R54] 比较两个文件
来源：http://xjh.yonumen.top

diff a.txt b.txt
来源：http://zdm.pengpengdd.cyou

[R55] 压缩与解压
来源：http://veu.zdbjq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://umw.jinqigfzy.top

[R56] 远程拷贝
来源：http://jxt.gotoacloud.top

scp file user@host:/path/
来源：http://llx.shangyingyoupin.top

[R57] 远程执行命令
来源：http://smd.ppjwa.cn

ssh user@host 'uptime'
来源：http://gzj.vqdsnc.cn

[R58] 下载文件
来源：http://qik.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://opk.xuanzx.com

[R59] 发 POST JSON
来源：http://hwz.sweek.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nqp.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://nbx.bjfxy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xfe.aizwys.cn

[R61] 磁盘占用
来源：http://pip.tanke756.top

df -h;  du -sh *
来源：http://lne.jyoumei.cn

[R62] 找最占空间的文件
来源：http://zpr.tanke756.top

du -ah . | sort -rh | head -10
来源：http://noy.guannengcc.top

[R63] 内存与进程
来源：http://cec.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://hxj.hnqzz.top

[R64] 结束进程
来源：http://hlh.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://cls.xingfuxueyuan.xyz

[R65] 查看端口占用
来源：http://nfz.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kwp.shzxlz.cn

[R66] 定时任务
来源：http://udf.dianchejie.cn

crontab -e;  crontab -l
来源：http://zey.xuanzx.com

[R67] 生成随机十六进制串
来源：http://gwg.sweek.top

openssl rand -hex 16
来源：http://jce.meibo888.top

[R68] 计算文件校验值
来源：http://oqy.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://pwe.vqdsnc.cn

[R69] 生成随机密码
来源：http://rfr.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://mjq.jiagoushi.top

[R70] 时间戳与互转
来源：http://ggx.52xcode.cn

date +%s;  date -d @1700000000
来源：http://fzm.tanke756.top

[R71] 日期格式化
来源：http://rpy.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://orm.yj20258.top

[R72] 等待端口就绪
来源：http://ahb.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tvn.daxiang520.top

[R73] 分割大日志
来源：http://pmo.redwolf501.top

split -l 1000 big.log part_
来源：http://scg.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://bin.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jpz.nanxinkj.top

[R75] 导出环境变量
来源：http://xqk.vehdjk.com

export PATH="$HOME/bin:$PATH"
来源：http://epx.pengpengdd.cyou

[R76] 使用临时文件
来源：http://bio.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pey.smart0.xyz

[R77] 读取用户输入
来源：http://zta.cqqwz.cn

read -rp "请输入: " ans
来源：http://top.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://hgc.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://jvj.sjlbkw.cn

[R79] 解析命令行选项
来源：http://kkd.cdnleiting.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qvi.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://ccl.zhengqikj.top

time ./run.sh
来源：http://qae.yuxming.cn

================================================================================
来源：http://utr.jlsjyb.cn

S. C / C++ 专题
来源：http://jlr.hesvh.cn

================================================================================
来源：http://vbi.hcnkem.com

[S01] C：Hello World
来源：http://oyq.jinyuanbaomall.cn

#include <stdio.h>
来源：http://wtk.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kwc.daria6918.cn

[S02] C：变量与格式化输出
来源：http://xff.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://lyh.zhoulong.xyz

[S03] C：读入整数
来源：http://pdy.ydzc1.top

int x; scanf("%d", &x);
来源：http://egt.nanxinkj.top

[S04] C：字符串复制
来源：http://eom.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://wik.tianlin.xyz

[S05] C：字符串长度
来源：http://wxz.shanyushiyangkeji.top

strlen(s)
来源：http://une.yangfankeji.com

[S06] C：字符串比较
来源：http://fpg.fehbvm.com

strcmp(a, b) == 0
来源：http://fyc.zdqjudy.top

[S07] C：数组遍历求和
来源：http://xnj.yfazqb.com


<!-- 参考信息 -->