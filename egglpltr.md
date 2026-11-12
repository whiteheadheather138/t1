代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cxk.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://ixp.jyoumei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lnr.52xcode.cn

[Q41] 多表连接
来源：http://ajs.birdmap.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jlt.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://mnx.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://dlv.yj20258888.top

[Q42] 连接条件附加过滤
来源：http://chr.zhixingplan.top

SELECT u.name, o.amount FROM users u
来源：http://pmh.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://czt.hnxiangtu.top

[Q43] 标量子查询
来源：http://rxa.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://att.guannengcc.top

[Q44] IN 子查询
来源：http://flz.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://skn.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://vkc.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zxn.sufxvd.cn

[Q46] NOT EXISTS 判断不存在
来源：http://whr.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zzk.shzxlz.cn

[Q47] 与平均值比较
来源：http://okt.fanxiaobao.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://spb.jinqigfzy.top

[Q48] CTE 公用表表达式
来源：http://qtd.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zlp.yongpay.top

SELECT * FROM t WHERE c > 5;
来源：http://iwp.shzxlz.cn

[Q49] 更新单行
来源：http://tww.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bzh.ehwqpu.com

[Q50] 批量更新
来源：http://vgt.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xfi.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://ywd.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xco.cdnleiting.top

[Q52] 删除指定行
来源：http://xwp.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://jpn.dashuyun.cn

[Q53] 按条件删除
来源：http://uux.yvedp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xyz.hcnkem.com

[Q54] 清空表
来源：http://jlo.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://yik.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://yxg.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vup.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://jfr.bjfxy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lql.fzhhl.top

[Q57] 行号
来源：http://yhe.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kfa.sjlbkw.cn

[Q58] 累计求和
来源：http://pub.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mzf.nanxinkj.top

[Q59] 分组内累计
来源：http://lrr.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cmk.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://ixm.zhiwuduotai.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gtt.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ude.yongpay.top

[Q61] 移动平均
来源：http://dxm.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gxl.dashuyun.cn

[Q62] 分组占比
来源：http://wyg.zdqjudy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gsl.redwolf501.top

[Q63] 开启事务
来源：http://fst.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://awh.jlsjyb.cn

[Q64] 提交事务
来源：http://uoi.chenzaomai.com

COMMIT;
来源：http://qsn.yj20258.top

[Q65] 回滚事务
来源：http://eib.fanxiaobao.xyz

ROLLBACK;
来源：http://jcr.52xcode.cn

[Q66] 行锁查询
来源：http://qji.zdbjq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://czn.cqqwz.cn

[Q67] 设置隔离级别
来源：http://aid.chenzaomai.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tfv.jinyuanbaomall.cn

[Q68] 保存点
来源：http://vln.316326.xyz

SAVEPOINT sp1;
来源：http://spq.fzhhl.top

ROLLBACK TO sp1;
来源：http://aqu.zhijiandao.cn

[Q69] 查看执行计划
来源：http://clj.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jgk.bjfxy.top

[Q70] 更新统计信息
来源：http://vgs.chenlongwang.top

ANALYZE TABLE users;
来源：http://jvu.sjlbkw.cn

[Q71] 查看建表语句
来源：http://ocx.meibo888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gnw.vqdsnc.cn

[Q72] 查看索引
来源：http://enb.cashguo.top

SHOW INDEX FROM users;
来源：http://hpt.zhongyouzk.top

[Q73] 查看表状态
来源：http://xga.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ccf.fengsongda.top

[Q74] 强制使用索引
来源：http://ftx.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://svv.havefunace.top

[Q75] 日期格式化
来源：http://zij.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vex.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tpx.yj202588.top

[Q76] 按天统计
来源：http://nes.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hmm.yueranfly.top

[Q77] 时间加减
来源：http://xjo.tianlin.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uos.iojbl.cn

[Q78] 当前时间
来源：http://qer.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oqu.9152youxi.cn

[Q79] 字符串拼接
来源：http://nny.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://npd.smart0.xyz

[Q80] 字符串截取
来源：http://ans.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pji.ydjk.org.cn

[Q81] 字符串替换
来源：http://uru.tarul.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ryq.shzxlz.cn

[Q82] 字符长度与字节长度
来源：http://jmk.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jdh.vehdjk.com

[Q83] 大小写转换
来源：http://cgz.jinghuilouyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://laq.9152youxi.cn

[Q84] 去除首尾空格
来源：http://ivn.zhaomingkeji.xyz

SELECT TRIM(name) FROM users;
来源：http://wvl.ybcxt.top

[Q85] 数值取整
来源：http://zyz.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sfz.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://mvi.snrcjt.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zii.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://hhr.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lbs.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://geg.zhoulong.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hjq.havefunace.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nev.ivvv.top

[Q89] 判断表是否存在
来源：http://dqm.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yop.jinghuilouyu.cn

[Q90] 生成序号列
来源：http://xxt.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pfy.chenzaomai.com

================================================================================
来源：http://fmf.jinqigfzy.top

R. Bash 专题
来源：http://mft.yuxming.cn

================================================================================
来源：http://rlu.yj202588.top

[R01] shebang 与严格模式
来源：http://hsq.uphjek.com

#!/usr/bin/env bash
来源：http://fcz.jianghu66.top

set -euo pipefail
来源：http://phm.cdnleiting.top

[R02] 变量赋值与使用
来源：http://dmd.chenlongwang.top

name="Tom"; echo "$name"
来源：http://wpa.hcnkem.com

[R03] 只读变量
来源：http://zrm.chenjidiqi.icu

readonly PI=3.14
来源：http://orp.redwolf501.top

[R04] 位置参数
来源：http://gpe.haohaochexian.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xtx.zhengqikj.top

[R05] 参数默认值
来源：http://aia.gogol.net.cn

name="${1:-default}"
来源：http://obl.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://uop.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hht.ybcxt.top

[R07] if 判断文件
来源：http://aoz.guannengcc.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fej.hammf.cn

[R08] 数值比较
来源：http://rlz.yj20258.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mkg.ydzc1.top

[R09] 字符串比较
来源：http://vkm.yvedp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vsc.yfazqb.com

[R10] 正则匹配
来源：http://ndf.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tvk.cucudq.cn

[R11] case 多分支
来源：http://gdv.c1oappe.top

case "$1" in
来源：http://ite.xziqi.cn

start) echo "启动" ;;
来源：http://zas.bjfxy.top

stop)  echo "停止" ;;
来源：http://msu.epnwcf.com

*)     echo "未知命令" ;;
来源：http://jqr.tarul.cn

esac
来源：http://xsh.cdnleiting.top

[R12] for 遍历文件
来源：http://zdv.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://zbx.xylfe.cn

[R13] for 计数循环
来源：http://nok.smart0.xyz

for i in {1..10}; do echo "$i"; done
来源：http://knm.jyoumei.cn

[R14] C 风格 for
来源：http://dhu.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tcv.pycfn.com

[R15] while 逐行读文件
来源：http://kai.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ggk.hnqzz.top

[R16] until 等待条件
来源：http://isc.ybcxt.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yza.xuetiantiany.cn

[R17] 数组定义与取值
来源：http://thc.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mpu.fehbvm.com

[R18] 遍历数组
来源：http://wip.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://upj.tanke756.top

[R19] 数组长度
来源：http://fyu.tanke756.top

echo "${#arr[@]}"
来源：http://foj.yuanzhike.top

[R20] 关联数组（字典）
来源：http://xxh.wangdashe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://egj.kuanghao11.cn

[R21] 字符串长度
来源：http://dwp.shanyushiyangkeji.top

echo "${#s}"
来源：http://whk.nwbrower.top

[R22] 截取子串
来源：http://alo.tianlin.xyz

echo "${s:0:5}"
来源：http://krs.yj20258.top

[R23] 字符串替换
来源：http://rlw.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kie.guowangkeji.top

[R24] 大小写转换
来源：http://bgq.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://hdh.ydjk.org.cn

[R25] 去后缀 / 去前缀
来源：http://eha.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://nbj.yueranfly.top

[R26] 命令替换
来源：http://ukv.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://tqt.vehdjk.com

[R27] 算术展开
来源：http://prl.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://vql.zhengqikj.top

[R28] 浮点运算
来源：http://qxr.feifeiyinyue.top

echo "scale=2; 10/3" | bc
来源：http://jaj.yuxming.cn

[R29] 定义函数
来源：http://lbs.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://opt.xinyue.icu

[R30] 函数返回状态码
来源：http://bdh.xziqi.cn

f() { return 0; }; f || echo "失败了"
来源：http://pnm.316326.xyz

[R31] 局部变量
来源：http://ghf.gogol.net.cn

f() { local x=1; echo "$x"; }
来源：http://tps.52xcode.cn

[R32] 参数个数校验
来源：http://guy.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jkg.ehwqpu.com

[R33] 捕获错误并提示行号
来源：http://bhd.hywenlv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qne.pengpengdd.cyou

[R34] 退出时清理
来源：http://zfb.cheryme.top

trap 'rm -f "$tmp"' EXIT
来源：http://zkw.xinyue.icu

[R35] 后台执行并等待
来源：http://xmg.andypj.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://fdx.sufxvd.cn

[R36] 并发执行多个任务
来源：http://sku.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zwe.guannengcc.top

[R37] 把输出赋给变量
来源：http://sww.gzhubu.top

files=$(ls -1)
来源：http://gzc.gaohongyu789.top

[R38] 管道串联
来源：http://jsu.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://shh.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://nym.dianchejie.cn

cmd > out.log 2>&1
来源：http://eph.xuetiantiany.cn

[R40] 追加写日志
来源：http://htw.zdqjudy.top

echo "log" >> out.log
来源：http://vzj.xuetiantiany.cn

[R41] 丢弃输出
来源：http://aen.hcnkem.com

cmd >/dev/null 2>&1
来源：http://uqq.yanxiufei.cn

[R42] 输入重定向
来源：http://hkj.fanxiaobao.xyz

wc -l < a.txt
来源：http://npv.zdqjudy.top

[R43] 按名字查找文件
来源：http://kcz.pycfn.com

find . -name "*.log" -type f
来源：http://yvs.hnqzz.top

[R44] 按修改时间查找
来源：http://qnw.daxiang520.top

find . -mtime -7 -type f
来源：http://qnz.ehwqpu.com

[R45] 批量删除
来源：http://gee.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://ygm.daria6918.cn

[R46] 递归替换文件内容
来源：http://tej.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ocj.daria6918.cn

[R47] sed 单行替换
来源：http://fop.9152youxi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://huu.pycfn.com

[R48] awk 取指定列
来源：http://zdi.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://zkb.zhixingplan.top

[R49] awk 带条件
来源：http://ylh.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qmo.guannengcc.top

[R50] awk 求和
来源：http://hwn.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xyo.yanxiufei.cn

[R51] 排序去重取前几
来源：http://pjf.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://nvb.nwbrower.top

[R52] 统计行数
来源：http://kor.yfazqb.com

wc -l a.txt
来源：http://pjo.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://bfc.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ily.mhx1999.top

[R54] 比较两个文件
来源：http://dro.zdbjq.cn

diff a.txt b.txt
来源：http://rgc.nanxinkj.top

[R55] 压缩与解压
来源：http://ybx.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://olb.jianghu66.top

[R56] 远程拷贝
来源：http://fgn.cheryme.top

scp file user@host:/path/
来源：http://noc.epnwcf.com

[R57] 远程执行命令
来源：http://gbt.nwbrower.top

ssh user@host 'uptime'
来源：http://hxs.yongpay.top

[R58] 下载文件
来源：http://cfi.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gai.sjlbkw.cn

[R59] 发 POST JSON
来源：http://pyk.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bnf.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://noo.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dom.xziqi.cn

[R61] 磁盘占用
来源：http://fcd.ywan-chungtsiang.top

df -h;  du -sh *
来源：http://bhk.pycfn.com

[R62] 找最占空间的文件
来源：http://nid.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://lml.cqqwz.cn

[R63] 内存与进程
来源：http://bvr.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://rvj.chenlongwang.top

[R64] 结束进程
来源：http://bam.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://vzw.yuanzhike.top

[R65] 查看端口占用
来源：http://vsr.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hzs.yj20258888.top

[R66] 定时任务
来源：http://kmj.xylfe.cn

crontab -e;  crontab -l
来源：http://qup.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://rwa.jlsjyb.cn

openssl rand -hex 16
来源：http://gtf.tianlin.xyz

[R68] 计算文件校验值
来源：http://avu.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://qgl.fengsongda.top

[R69] 生成随机密码
来源：http://ari.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://hpf.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://adm.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://url.jlsjyb.cn

[R71] 日期格式化
来源：http://msy.xylfe.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sss.uphjek.com

[R72] 等待端口就绪
来源：http://oxf.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ewn.jinghuilouyu.cn

[R73] 分割大日志
来源：http://smr.shangyingyoupin.top

split -l 1000 big.log part_
来源：http://qcm.yfazqb.com

[R74] 批量重命名
来源：http://hdp.aibaodan.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pus.zhongyouzk.top

[R75] 导出环境变量
来源：http://rav.wangshuangyany.cn

export PATH="$HOME/bin:$PATH"
来源：http://hba.uphjek.com

[R76] 使用临时文件
来源：http://xzr.zhaomingkeji.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vji.zhoulong.xyz

[R77] 读取用户输入
来源：http://bfr.yj20258.top

read -rp "请输入: " ans
来源：http://bmu.zhoulong.xyz

[R78] 交互式菜单
来源：http://tkv.52xcode.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tej.dashuyun.cn

[R79] 解析命令行选项
来源：http://lip.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ycp.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://yfr.haohaochexian.top

time ./run.sh
来源：http://qgq.uphjek.com

================================================================================
来源：http://wpa.yj202588.top

S. C / C++ 专题
来源：http://puc.bjfxy.top

================================================================================
来源：http://hqu.meibo888.top

[S01] C：Hello World
来源：http://hge.316326.xyz

#include <stdio.h>
来源：http://gsl.pengpengdd.cyou

int main(void) { printf("Hello\n"); return 0; }
来源：http://fbo.cucudq.cn

[S02] C：变量与格式化输出
来源：http://xjg.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://xtp.xinyue.icu

[S03] C：读入整数
来源：http://hfd.daxiang520.top

int x; scanf("%d", &x);
来源：http://mzw.yj20258888.top

[S04] C：字符串复制
来源：http://yub.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://vch.pycfn.com

[S05] C：字符串长度
来源：http://sxy.gzhubu.top

strlen(s)
来源：http://pxe.pycfn.com

[S06] C：字符串比较
来源：http://pmd.gzhubu.top

strcmp(a, b) == 0
来源：http://nxq.ydzc1.top

[S07] C：数组遍历求和
来源：http://zop.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://maz.316326.xyz

[S08] C：动态内存分配与释放
来源：http://suk.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aaw.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://mpk.dianchejie.cn


<!-- 参考信息 -->