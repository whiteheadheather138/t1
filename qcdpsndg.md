代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qek.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wzr.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jma.ehwqpu.com

[Q41] 多表连接
来源：http://lfb.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sod.hywenlv.cn

JOIN users u ON u.id = o.user_id
来源：http://kyj.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://rit.cashguo.top

[Q42] 连接条件附加过滤
来源：http://tat.chenjidiqi.icu

SELECT u.name, o.amount FROM users u
来源：http://hhy.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://txv.zhijiandao.cn

[Q43] 标量子查询
来源：http://skz.feifeiyinyue.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rhu.pengpengdd.cyou

[Q44] IN 子查询
来源：http://uij.iojbl.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zho.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://cln.haohaochexian.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fzq.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://uqq.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qcs.bbcook.cn

[Q47] 与平均值比较
来源：http://lck.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vde.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://vpc.yuanzhike.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qqt.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://foy.jlsjyb.cn

[Q49] 更新单行
来源：http://ykz.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wau.chenjidiqi.icu

[Q50] 批量更新
来源：http://dwl.zdqjudy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rqb.yvedp.cn

[Q51] 用子查询更新
来源：http://qvw.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qxb.sxryk.cn

[Q52] 删除指定行
来源：http://ljg.9152youxi.cn

DELETE FROM users WHERE id = 10;
来源：http://edt.hysaishi.cn

[Q53] 按条件删除
来源：http://sjc.pengpengdd.cyou

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ioo.jqgfzy.top

[Q54] 清空表
来源：http://fmc.hesvh.cn

TRUNCATE TABLE logs;
来源：http://ldl.gzhubu.top

[Q55] 排名（并列占位）
来源：http://hzg.tarul.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hqd.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://bsc.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hup.kuanghao11.cn

[Q57] 行号
来源：http://jlm.fanxiaobao.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ehs.mhx1999.top

[Q58] 累计求和
来源：http://ent.ppjwa.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qga.jqgufenzy.top

[Q59] 分组内累计
来源：http://yfr.cqqwz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rub.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://pcf.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gtj.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://quu.shzxlz.cn

[Q61] 移动平均
来源：http://anu.fanxiaobao.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ndw.andypj.xyz

[Q62] 分组占比
来源：http://qeo.c1oappe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vvf.shzxlz.cn

[Q63] 开启事务
来源：http://qeg.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nfo.xziqi.cn

[Q64] 提交事务
来源：http://zel.jinghuilouyu.cn

COMMIT;
来源：http://urm.tarul.cn

[Q65] 回滚事务
来源：http://lzo.nanxinkj.top

ROLLBACK;
来源：http://wvg.daria6918.cn

[Q66] 行锁查询
来源：http://ovr.gzhubu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bdc.shanyushiyangtech.top

[Q67] 设置隔离级别
来源：http://jeq.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ffr.gotoacloud.top

[Q68] 保存点
来源：http://jrr.9152youxi.cn

SAVEPOINT sp1;
来源：http://fyk.nwbrower.top

ROLLBACK TO sp1;
来源：http://qyk.jinqigufen.top

[Q69] 查看执行计划
来源：http://qpg.vqdsnc.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ypt.shuidangran.top

[Q70] 更新统计信息
来源：http://fuv.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://vev.jianghu66.top

[Q71] 查看建表语句
来源：http://kzp.iojbl.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bqx.ehwqpu.com

[Q72] 查看索引
来源：http://mep.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://tnt.smart0.xyz

[Q73] 查看表状态
来源：http://eqq.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bdw.yuanzhike.top

[Q74] 强制使用索引
来源：http://biv.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lqz.shanyushiyangkeji.top

[Q75] 日期格式化
来源：http://ikb.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tuz.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://opj.pycfn.com

[Q76] 按天统计
来源：http://eiz.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://scq.epnwcf.com

[Q77] 时间加减
来源：http://bxd.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://giz.haohaochexian.top

[Q78] 当前时间
来源：http://ntw.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cpa.yongpay.top

[Q79] 字符串拼接
来源：http://zeq.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ckr.dianchejie.cn

[Q80] 字符串截取
来源：http://cjg.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hjh.316326.xyz

[Q81] 字符串替换
来源：http://yap.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ara.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://khg.dashuyun.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://meu.redwolf501.top

[Q83] 大小写转换
来源：http://mdq.cheryme.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qha.redwolf501.top

[Q84] 去除首尾空格
来源：http://wzj.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://spi.shzxlz.cn

[Q85] 数值取整
来源：http://hqf.ivvv.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lrv.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://hbq.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://unc.jinghuilouyu.cn

[Q87] JSON 字段做条件
来源：http://lbf.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aam.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://iso.wangshuangyany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zij.yuxming.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mlp.52xcode.cn

[Q89] 判断表是否存在
来源：http://mne.jqgfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nqh.cheryme.top

[Q90] 生成序号列
来源：http://xbf.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://atc.tarul.cn

================================================================================
来源：http://smw.pengpengdd.cyou

R. Bash 专题
来源：http://pjk.shanyushiyangkeji.top

================================================================================
来源：http://vpb.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://ebi.cashguo.top

#!/usr/bin/env bash
来源：http://cye.dianchejie.cn

set -euo pipefail
来源：http://gfx.gotoacloud.top

[R02] 变量赋值与使用
来源：http://fck.yueranfly.top

name="Tom"; echo "$name"
来源：http://kkb.yongpay.top

[R03] 只读变量
来源：http://ceu.aibaodan.cn

readonly PI=3.14
来源：http://bvx.jqgufenzy.top

[R04] 位置参数
来源：http://frn.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://deh.jinqigufen.top

[R05] 参数默认值
来源：http://ukl.fzhhl.top

name="${1:-default}"
来源：http://fqr.tian-w.cn

[R06] 判断命令是否存在
来源：http://dgz.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://krj.shanyushiyangtech.top

[R07] if 判断文件
来源：http://jot.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qxm.gzhubu.top

[R08] 数值比较
来源：http://qvq.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://pxn.daxiang520.top

[R09] 字符串比较
来源：http://cxi.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://unh.yj20258.top

[R10] 正则匹配
来源：http://ywo.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uat.cucudq.cn

[R11] case 多分支
来源：http://zsv.xylfe.cn

case "$1" in
来源：http://vtp.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://wwo.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://sci.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://ott.mhx1999.top

esac
来源：http://fai.daria6918.cn

[R12] for 遍历文件
来源：http://iak.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://csd.yuxming.cn

[R13] for 计数循环
来源：http://wlm.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://mfw.bjfxy.top

[R14] C 风格 for
来源：http://axb.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bwe.shuidangran.top

[R15] while 逐行读文件
来源：http://eft.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hqf.epnwcf.com

[R16] until 等待条件
来源：http://ese.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sci.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://rhi.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://lha.zhoulong.xyz

[R18] 遍历数组
来源：http://osw.sysykeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://umb.nwbrower.top

[R19] 数组长度
来源：http://hxs.cdnleiting.top

echo "${#arr[@]}"
来源：http://bek.redwolf501.top

[R20] 关联数组（字典）
来源：http://mnl.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dsq.52xcode.cn

[R21] 字符串长度
来源：http://wsr.ctjpmb.com

echo "${#s}"
来源：http://uyc.shanyushiyangkeji.top

[R22] 截取子串
来源：http://muo.ydzc1.top

echo "${s:0:5}"
来源：http://pfl.smart0.xyz

[R23] 字符串替换
来源：http://cvx.ydjk.org.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rkr.guowangkeji.top

[R24] 大小写转换
来源：http://ugy.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://meg.quarkkingdee.top

[R25] 去后缀 / 去前缀
来源：http://tnc.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jbm.chenzaomai.com

[R26] 命令替换
来源：http://bnf.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://wjw.sjlbkw.cn

[R27] 算术展开
来源：http://tmt.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://wua.pengpengdd.cyou

[R28] 浮点运算
来源：http://dht.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://cji.andypj.xyz

[R29] 定义函数
来源：http://vsy.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dai.vehdjk.com

[R30] 函数返回状态码
来源：http://gjc.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://igo.sjlbkw.cn

[R31] 局部变量
来源：http://hak.dashuyun.cn

f() { local x=1; echo "$x"; }
来源：http://obd.bbcook.cn

[R32] 参数个数校验
来源：http://xrk.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gip.xuanzx.com

[R33] 捕获错误并提示行号
来源：http://tzx.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fme.pengpengdd.cyou

[R34] 退出时清理
来源：http://qdd.aizwys.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lft.mhx1999.top

[R35] 后台执行并等待
来源：http://xju.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ari.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://nih.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yoe.jinqigufen.top

[R37] 把输出赋给变量
来源：http://oqt.zhaomingkeji.xyz

files=$(ls -1)
来源：http://eti.birdmap.top

[R38] 管道串联
来源：http://jps.0kj1m.cn

cat a.txt | grep -i error | wc -l
来源：http://gqk.hnqzz.top

[R39] 重定向标准输出与错误
来源：http://iid.jyoumei.cn

cmd > out.log 2>&1
来源：http://bfv.fanxiaobao.xyz

[R40] 追加写日志
来源：http://wtt.hcnkem.com

echo "log" >> out.log
来源：http://tat.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://sfq.fktsv.cn

cmd >/dev/null 2>&1
来源：http://waj.cqqwz.cn

[R42] 输入重定向
来源：http://okz.hcnkem.com

wc -l < a.txt
来源：http://bxw.gaohongyu789.top

[R43] 按名字查找文件
来源：http://zjx.jinqigfzy.top

find . -name "*.log" -type f
来源：http://dub.wangdashe.top

[R44] 按修改时间查找
来源：http://djt.yuxming.cn

find . -mtime -7 -type f
来源：http://ufb.bjfxy.top

[R45] 批量删除
来源：http://bbj.uphjek.com

find . -name "*.tmp" -delete
来源：http://opg.hywenlv.cn

[R46] 递归替换文件内容
来源：http://zjk.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ilh.c1oappe.top

[R47] sed 单行替换
来源：http://flm.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gzg.316326.xyz

[R48] awk 取指定列
来源：http://ygs.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://upo.tianlin.xyz

[R49] awk 带条件
来源：http://oze.chenlongwang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://icg.shzxlz.cn

[R50] awk 求和
来源：http://xpg.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://lqq.yueranfly.top

[R51] 排序去重取前几
来源：http://jjo.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pxq.smart0.xyz

[R52] 统计行数
来源：http://llo.aizwys.cn

wc -l a.txt
来源：http://phd.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://kso.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eid.mhx1999.top

[R54] 比较两个文件
来源：http://xhz.sufxvd.cn

diff a.txt b.txt
来源：http://gnl.xylfe.cn

[R55] 压缩与解压
来源：http://btj.ywan-chungtsiang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pqu.mhx1999.top

[R56] 远程拷贝
来源：http://kji.uphjek.com

scp file user@host:/path/
来源：http://mbe.ydjk.org.cn

[R57] 远程执行命令
来源：http://oqe.cucudq.cn

ssh user@host 'uptime'
来源：http://kra.hfpthk.cn

[R58] 下载文件
来源：http://een.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fxo.yj202588.top

[R59] 发 POST JSON
来源：http://nwc.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://skw.fehbvm.com

[R60] 只看 HTTP 状态码
来源：http://anw.nwbrower.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://psj.sysykeji.top

[R61] 磁盘占用
来源：http://sly.svipenyu.cn

df -h;  du -sh *
来源：http://osh.hcnkem.com

[R62] 找最占空间的文件
来源：http://rap.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://vgw.zhengqikj.top

[R63] 内存与进程
来源：http://lwe.shanyushiyangkeji.top

free -h;  ps aux | grep nginx
来源：http://bzl.yj20258888.top

[R64] 结束进程
来源：http://vns.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://nbf.yj202588.top

[R65] 查看端口占用
来源：http://uhy.guowangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://drr.uphjek.com

[R66] 定时任务
来源：http://ufg.jqgfzy.top

crontab -e;  crontab -l
来源：http://whk.birdmap.top

[R67] 生成随机十六进制串
来源：http://mgi.cheryme.top

openssl rand -hex 16
来源：http://tlx.yj20258888.top

[R68] 计算文件校验值
来源：http://adc.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://mbp.zhaomingkeji.xyz

[R69] 生成随机密码
来源：http://uot.mhx1999.top

head -c 16 /dev/urandom | base64
来源：http://nkq.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://djn.tarul.cn

date +%s;  date -d @1700000000
来源：http://xmg.zhijiandao.cn

[R71] 日期格式化
来源：http://nrf.pengpengdd.cyou

date +"%Y-%m-%d %H:%M:%S"
来源：http://yct.hesvh.cn

[R72] 等待端口就绪
来源：http://vqc.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eyr.316326.xyz

[R73] 分割大日志
来源：http://gso.chenzaomai.com

split -l 1000 big.log part_
来源：http://wdd.chenjidiqi.icu

[R74] 批量重命名
来源：http://cox.ywan-chungtsiang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tdk.xinyue.icu

[R75] 导出环境变量
来源：http://bew.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://cuq.wangshuangyany.cn

[R76] 使用临时文件
来源：http://hgz.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wek.xylfe.cn

[R77] 读取用户输入
来源：http://ruf.316326.xyz

read -rp "请输入: " ans
来源：http://woa.cdnleiting.top

[R78] 交互式菜单
来源：http://ffs.ehwqpu.com

select opt in a b c; do echo "$opt"; break; done
来源：http://jiy.52xcode.cn

[R79] 解析命令行选项
来源：http://dub.yangfankeji.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vxy.uphjek.com

[R80] 查看脚本执行耗时
来源：http://rhf.jinqigufen.top

time ./run.sh
来源：http://fin.sufxvd.cn

================================================================================
来源：http://dzi.gzhubu.top

S. C / C++ 专题
来源：http://dbz.daria6918.cn

================================================================================
来源：http://ynb.iojbl.cn

[S01] C：Hello World
来源：http://rpy.jqgufenzy.top

#include <stdio.h>
来源：http://cmi.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xad.mhx1999.top

[S02] C：变量与格式化输出
来源：http://oiy.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://vml.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://ccw.ctjpmb.com

int x; scanf("%d", &x);
来源：http://jlu.ybcxt.top

[S04] C：字符串复制
来源：http://sjw.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://zdg.tarul.cn

[S05] C：字符串长度
来源：http://fng.yongpay.top

strlen(s)
来源：http://olo.cdnleiting.top

[S06] C：字符串比较
来源：http://ihf.yuanzhike.top

strcmp(a, b) == 0
来源：http://faw.cqqwz.cn

[S07] C：数组遍历求和
来源：http://pqq.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tmb.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://ptx.yongpay.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ulq.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://gan.hongshengwenyu.top


<!-- 参考信息 -->