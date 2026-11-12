代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://rjt.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://web.yuanzhike.top

JOIN products p ON p.id = o.product_id;
来源：http://ufr.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://occ.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://fhg.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://opu.zhixingplan.top

[Q43] 标量子查询
来源：http://znr.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://quu.sjlbkw.cn

[Q44] IN 子查询
来源：http://axf.guannengcc.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sue.fktsv.cn

[Q45] EXISTS 判断存在
来源：http://sqi.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jmq.chenjidiqi.icu

[Q46] NOT EXISTS 判断不存在
来源：http://kjy.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rwt.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://rxr.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rkd.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://kiu.hammf.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vsa.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://tno.vqdsnc.cn

[Q49] 更新单行
来源：http://bxv.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fxb.yongpay.top

[Q50] 批量更新
来源：http://jmu.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nxi.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://yoq.snrcjt.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rfd.chenjidiqi.icu

[Q52] 删除指定行
来源：http://sfv.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://rzg.cqqwz.cn

[Q53] 按条件删除
来源：http://kmu.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://swf.zhoulong.xyz

[Q54] 清空表
来源：http://glg.daria6918.cn

TRUNCATE TABLE logs;
来源：http://pgm.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://vjw.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mju.cucudq.cn

[Q56] 密集排名（并列不占位）
来源：http://ofs.jinyuanbaomall.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zpl.nwbrower.top

[Q57] 行号
来源：http://aab.ppjwa.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hgg.fktsv.cn

[Q58] 累计求和
来源：http://yib.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jhf.jqgufenzy.top

[Q59] 分组内累计
来源：http://oiz.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nhb.c1oappe.top

[Q60] 取上一行 / 下一行
来源：http://lha.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qow.andypj.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ejp.fzhhl.top

[Q61] 移动平均
来源：http://qqn.haohaochexian.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uqw.uphjek.com

[Q62] 分组占比
来源：http://kcu.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yfp.yanxiufei.cn

[Q63] 开启事务
来源：http://saz.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gfe.yvedp.cn

[Q64] 提交事务
来源：http://cgf.tanke756.top

COMMIT;
来源：http://sqw.jlsjyb.cn

[Q65] 回滚事务
来源：http://wou.jinqigfzy.top

ROLLBACK;
来源：http://elw.fengsongda.top

[Q66] 行锁查询
来源：http://pip.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lrw.sweek.top

[Q67] 设置隔离级别
来源：http://cgs.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qmi.yueranfly.top

[Q68] 保存点
来源：http://lcu.sjlbkw.cn

SAVEPOINT sp1;
来源：http://nfm.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://aue.vqdsnc.cn

[Q69] 查看执行计划
来源：http://yoh.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://imu.vqdsnc.cn

[Q70] 更新统计信息
来源：http://xee.xinyue.icu

ANALYZE TABLE users;
来源：http://lzd.jinqigufen.top

[Q71] 查看建表语句
来源：http://mpd.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gcv.c1oappe.top

[Q72] 查看索引
来源：http://dpo.yj20258.top

SHOW INDEX FROM users;
来源：http://eqd.cqqwz.cn

[Q73] 查看表状态
来源：http://uru.snrcjt.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ybr.jinqigufen.top

[Q74] 强制使用索引
来源：http://ofn.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bps.zdbjq.cn

[Q75] 日期格式化
来源：http://pti.ehwqpu.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sxg.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xim.zhongyouzk.top

[Q76] 按天统计
来源：http://isv.svipenyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cnx.guowangkeji.top

[Q77] 时间加减
来源：http://cvg.yvedp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jon.sweek.top

[Q78] 当前时间
来源：http://sme.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pmr.ybcxt.top

[Q79] 字符串拼接
来源：http://lup.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sbi.yueranfly.top

[Q80] 字符串截取
来源：http://wyf.ybcxt.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xre.gaohongyu789.top

[Q81] 字符串替换
来源：http://tca.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://snw.dashuyun.cn

[Q82] 字符长度与字节长度
来源：http://paw.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://arq.tianlin.xyz

[Q83] 大小写转换
来源：http://zur.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rqq.smart0.xyz

[Q84] 去除首尾空格
来源：http://qys.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://osp.yj20258888.top

[Q85] 数值取整
来源：http://kpk.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fnl.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://rtp.wangshuangyany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nlo.sysykeji.top

[Q87] JSON 字段做条件
来源：http://oan.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ift.yuxming.cn

[Q88] 行转列（条件聚合）
来源：http://cya.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cgf.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://avb.xuetiantiany.cn

[Q89] 判断表是否存在
来源：http://ulh.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cxa.snrcjt.cn

[Q90] 生成序号列
来源：http://ivt.xingfuxueyuan.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vho.bbcook.cn

================================================================================
来源：http://qxa.cheryme.top

R. Bash 专题
来源：http://ojp.xylfe.cn

================================================================================
来源：http://bby.fzhhl.top

[R01] shebang 与严格模式
来源：http://wji.aizwys.cn

#!/usr/bin/env bash
来源：http://auk.jinghuilouyu.cn

set -euo pipefail
来源：http://qte.aibaodan.cn

[R02] 变量赋值与使用
来源：http://aib.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://bcp.daxiang520.top

[R03] 只读变量
来源：http://neh.zhongyouzk.top

readonly PI=3.14
来源：http://mak.haohaochexian.top

[R04] 位置参数
来源：http://cuc.ydzc1.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dbg.yj20258888.top

[R05] 参数默认值
来源：http://wiz.hongshengwenyu.top

name="${1:-default}"
来源：http://bwv.fehbvm.com

[R06] 判断命令是否存在
来源：http://kmj.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://znk.bjfxy.top

[R07] if 判断文件
来源：http://chr.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jwr.bbcook.cn

[R08] 数值比较
来源：http://few.0kj1m.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ztp.zhoulong.xyz

[R09] 字符串比较
来源：http://wqo.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hsl.zhixingplan.top

[R10] 正则匹配
来源：http://sgn.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dob.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://vjv.yj20258888.top

case "$1" in
来源：http://qym.yonumen.top

start) echo "启动" ;;
来源：http://gzd.fehbvm.com

stop)  echo "停止" ;;
来源：http://asj.ivvv.top

*)     echo "未知命令" ;;
来源：http://foa.zhoulong.xyz

esac
来源：http://qmp.gotoacloud.top

[R12] for 遍历文件
来源：http://zvo.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://yqw.ydjk.org.cn

[R13] for 计数循环
来源：http://kjp.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://qmx.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://vaf.gzhubu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hwc.yj20258888.top

[R15] while 逐行读文件
来源：http://jgi.andypj.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rov.kuanghao11.cn

[R16] until 等待条件
来源：http://ekz.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jeb.ctjpmb.com

[R17] 数组定义与取值
来源：http://dph.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://ebo.jqgufenzy.top

[R18] 遍历数组
来源：http://uch.pengpengdd.cyou

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lna.xuetiantiany.cn

[R19] 数组长度
来源：http://qug.aizwys.cn

echo "${#arr[@]}"
来源：http://zax.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://iup.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vhp.316326.xyz

[R21] 字符串长度
来源：http://ogt.yfazqb.com

echo "${#s}"
来源：http://dcw.jinqigfzy.top

[R22] 截取子串
来源：http://rqp.nwbrower.top

echo "${s:0:5}"
来源：http://yit.aizwys.cn

[R23] 字符串替换
来源：http://yqx.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pzn.yj20258.top

[R24] 大小写转换
来源：http://ago.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://wny.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://fxx.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://yyd.hfpthk.cn

[R26] 命令替换
来源：http://qlo.yvedp.cn

now=$(date +%F); echo "$now"
来源：http://hhs.pengpengdd.cyou

[R27] 算术展开
来源：http://sjw.yongpay.top

echo $((1 + 2 * 3))
来源：http://gxp.ppjwa.cn

[R28] 浮点运算
来源：http://lhz.yanxiufei.cn

echo "scale=2; 10/3" | bc
来源：http://aax.shanyushiyangtech.top

[R29] 定义函数
来源：http://lbk.zdqjudy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ozh.c1oappe.top

[R30] 函数返回状态码
来源：http://jxy.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://qpe.sufxvd.cn

[R31] 局部变量
来源：http://lfa.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://jdw.jlsjyb.cn

[R32] 参数个数校验
来源：http://dff.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xig.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://mge.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://frb.jqgfzy.top

[R34] 退出时清理
来源：http://dez.nwbrower.top

trap 'rm -f "$tmp"' EXIT
来源：http://nte.yvedp.cn

[R35] 后台执行并等待
来源：http://dvd.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://idv.jyoumei.cn

[R36] 并发执行多个任务
来源：http://fts.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lhf.fengsongda.top

[R37] 把输出赋给变量
来源：http://wjb.yj20258888.top

files=$(ls -1)
来源：http://ipv.hesvh.cn

[R38] 管道串联
来源：http://hyt.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://blu.jqgufenzy.top

[R39] 重定向标准输出与错误
来源：http://jmy.gaohongyu789.top

cmd > out.log 2>&1
来源：http://avt.fehbvm.com

[R40] 追加写日志
来源：http://fhe.zycfv.cn

echo "log" >> out.log
来源：http://ubq.zhiwuduotai.top

[R41] 丢弃输出
来源：http://ymy.ybcxt.top

cmd >/dev/null 2>&1
来源：http://lvo.sxryk.cn

[R42] 输入重定向
来源：http://djo.chenlongwang.top

wc -l < a.txt
来源：http://jqu.shangyingyoupin.top

[R43] 按名字查找文件
来源：http://oqh.nanxuanxn.top

find . -name "*.log" -type f
来源：http://pay.sysykeji.top

[R44] 按修改时间查找
来源：http://wwd.cqqwz.cn

find . -mtime -7 -type f
来源：http://xpf.ybcxt.top

[R45] 批量删除
来源：http://ugp.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://ncg.xziqi.cn

[R46] 递归替换文件内容
来源：http://jrr.9152youxi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yhl.meibo888.top

[R47] sed 单行替换
来源：http://yej.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://sez.jinqigfzy.top

[R48] awk 取指定列
来源：http://mlu.shzxlz.cn

awk '{print $1, $3}' a.txt
来源：http://ggq.zhiwuduotai.top

[R49] awk 带条件
来源：http://imf.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kph.cheryme.top

[R50] awk 求和
来源：http://wou.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://eip.haohaochexian.top

[R51] 排序去重取前几
来源：http://ulz.gaohongyu789.top

sort a.txt | uniq -c | sort -rn | head
来源：http://snx.shzxlz.cn

[R52] 统计行数
来源：http://kvq.yanxiufei.cn

wc -l a.txt
来源：http://dtc.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://qwh.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tae.gogol.net.cn

[R54] 比较两个文件
来源：http://pjc.nwbrower.top

diff a.txt b.txt
来源：http://ymu.hcnkem.com

[R55] 压缩与解压
来源：http://jox.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hul.yfazqb.com

[R56] 远程拷贝
来源：http://lfj.tian-w.cn

scp file user@host:/path/
来源：http://cmb.zhengqikj.top

[R57] 远程执行命令
来源：http://dxm.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://ljy.jianghu66.top

[R58] 下载文件
来源：http://wbj.meibo888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rtu.xingfuxueyuan.xyz

[R59] 发 POST JSON
来源：http://drf.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rek.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://woh.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qmd.pengpengdd.cyou

[R61] 磁盘占用
来源：http://got.chenzaomai.com

df -h;  du -sh *
来源：http://hjr.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://xen.tanke756.top

du -ah . | sort -rh | head -10
来源：http://qeq.redwolf501.top

[R63] 内存与进程
来源：http://olz.yj202588.top

free -h;  ps aux | grep nginx
来源：http://yop.guannengcc.top

[R64] 结束进程
来源：http://fbc.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://dqd.snrcjt.cn

[R65] 查看端口占用
来源：http://cwj.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xna.ivvv.top

[R66] 定时任务
来源：http://gxa.jinqigfzy.top

crontab -e;  crontab -l
来源：http://efn.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://ied.hnxiangtu.top

openssl rand -hex 16
来源：http://qwq.jianghu66.top

[R68] 计算文件校验值
来源：http://zrq.hesvh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vvn.havefunace.top

[R69] 生成随机密码
来源：http://qkv.hnqzz.top

head -c 16 /dev/urandom | base64
来源：http://kcb.cashguo.top

[R70] 时间戳与互转
来源：http://ruz.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://pog.zhongyouzk.top

[R71] 日期格式化
来源：http://qov.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eda.wangdashe.top

[R72] 等待端口就绪
来源：http://vwi.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mvj.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://xwn.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://dea.xziqi.cn

[R74] 批量重命名
来源：http://sls.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xhj.guannengcc.top

[R75] 导出环境变量
来源：http://hwm.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://lmd.cdnleiting.top

[R76] 使用临时文件
来源：http://yrb.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ghb.snrcjt.cn

[R77] 读取用户输入
来源：http://ynp.sufxvd.cn

read -rp "请输入: " ans
来源：http://mac.vehdjk.com

[R78] 交互式菜单
来源：http://yuv.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://vjs.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://rhu.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://acc.tarul.cn

[R80] 查看脚本执行耗时
来源：http://cdi.sysykeji.top

time ./run.sh
来源：http://ldo.nwbrower.top

================================================================================
来源：http://unn.nanxuanxn.top

S. C / C++ 专题
来源：http://lwd.xylfe.cn

================================================================================
来源：http://giw.nanxinkj.top

[S01] C：Hello World
来源：http://jlb.wangshuangyany.cn

#include <stdio.h>
来源：http://ysj.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://egi.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://gsn.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://txg.birdmap.top

[S03] C：读入整数
来源：http://shb.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://mrp.ctjpmb.com

[S04] C：字符串复制
来源：http://gdw.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://oic.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://blr.hammf.cn

strlen(s)
来源：http://qbg.nwbrower.top

[S06] C：字符串比较
来源：http://koz.wangdashe.top

strcmp(a, b) == 0
来源：http://idv.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://rel.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hji.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://xhl.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jel.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://jhh.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hmj.zhengqikj.top

[S10] C：指针与解引用
来源：http://bem.316326.xyz

int *p = &a;  *p = 5;
来源：http://jfq.jqgufenzy.top

[S11] C：逐行读文件
来源：http://ume.jiagoushi.top


<!-- 参考信息 -->