代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://oyt.xinyue.icu

JOIN users u ON u.id = o.user_id
来源：http://ejg.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://ohy.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://akk.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://slh.haohaochexian.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://orb.hysaishi.cn

[Q43] 标量子查询
来源：http://wjf.ybcxt.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wqs.zhongyouzk.top

[Q44] IN 子查询
来源：http://ugu.hywenlv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ajr.sysykeji.top

[Q45] EXISTS 判断存在
来源：http://pue.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pqg.c1oappe.top

[Q46] NOT EXISTS 判断不存在
来源：http://hwi.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dtf.cucudq.cn

[Q47] 与平均值比较
来源：http://scp.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hxa.fanxiaobao.xyz

[Q48] CTE 公用表表达式
来源：http://gfl.zhoulong.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ika.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://ubo.feifeiyinyue.top

[Q49] 更新单行
来源：http://dpf.jlsjyb.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rom.yangfankeji.com

[Q50] 批量更新
来源：http://ict.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://azp.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://zdf.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kxz.hesvh.cn

[Q52] 删除指定行
来源：http://xgb.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://qnu.9152youxi.cn

[Q53] 按条件删除
来源：http://apf.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://maf.guowangkeji.top

[Q54] 清空表
来源：http://lle.tarul.cn

TRUNCATE TABLE logs;
来源：http://chi.aibaodan.cn

[Q55] 排名（并列占位）
来源：http://pbf.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zaf.yangfankeji.com

[Q56] 密集排名（并列不占位）
来源：http://wlb.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://szr.shanyushiyangkeji.top

[Q57] 行号
来源：http://fxs.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://trj.yangfankeji.com

[Q58] 累计求和
来源：http://iux.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qat.daxiang520.top

[Q59] 分组内累计
来源：http://bab.aibaodan.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vbz.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://cdv.jianghu66.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://irs.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jrb.zdbjq.cn

[Q61] 移动平均
来源：http://gbn.sysykeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://quw.jyoumei.cn

[Q62] 分组占比
来源：http://edn.fehbvm.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://otd.chenlongwang.top

[Q63] 开启事务
来源：http://mzl.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zif.zdbjq.cn

[Q64] 提交事务
来源：http://ccw.aibaodan.cn

COMMIT;
来源：http://xwc.havefunace.top

[Q65] 回滚事务
来源：http://hqx.uphjek.com

ROLLBACK;
来源：http://uku.fengsongda.top

[Q66] 行锁查询
来源：http://frd.nanxinkj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kps.cdnleiting.top

[Q67] 设置隔离级别
来源：http://zgy.ctjpmb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vgd.jinqigfzy.top

[Q68] 保存点
来源：http://ozu.shzxlz.cn

SAVEPOINT sp1;
来源：http://typ.smart0.xyz

ROLLBACK TO sp1;
来源：http://bpx.smart0.xyz

[Q69] 查看执行计划
来源：http://cwz.xingfuxueyuan.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uoe.gaohongyu789.top

[Q70] 更新统计信息
来源：http://dqd.gzhubu.top

ANALYZE TABLE users;
来源：http://rif.zdbjq.cn

[Q71] 查看建表语句
来源：http://oag.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cva.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://ioh.hongshengwenyu.top

SHOW INDEX FROM users;
来源：http://iqc.pycfn.com

[Q73] 查看表状态
来源：http://fjm.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://ztw.xingfuxueyuan.xyz

[Q74] 强制使用索引
来源：http://tey.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ckl.nwbrower.top

[Q75] 日期格式化
来源：http://mxc.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bag.xylfe.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://njc.xinyue.icu

[Q76] 按天统计
来源：http://rzu.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oov.nanxuanxn.top

[Q77] 时间加减
来源：http://zfe.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://htj.chenlongwang.top

[Q78] 当前时间
来源：http://kmt.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fqm.shzxlz.cn

[Q79] 字符串拼接
来源：http://nnw.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pvv.gaohongyu789.top

[Q80] 字符串截取
来源：http://sqi.jlsjyb.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://osn.yvedp.cn

[Q81] 字符串替换
来源：http://mvs.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dlb.svipenyu.cn

[Q82] 字符长度与字节长度
来源：http://tta.yueranfly.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kcd.ivvv.top

[Q83] 大小写转换
来源：http://ckp.hnxiangtu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fty.yuanzhike.top

[Q84] 去除首尾空格
来源：http://jdi.hfpthk.cn

SELECT TRIM(name) FROM users;
来源：http://vfz.chenjidiqi.icu

[Q85] 数值取整
来源：http://igv.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tqa.chenlongwang.top

[Q86] 读取 JSON 字段
来源：http://jyo.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://job.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://hvf.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ezk.hcnkem.com

[Q88] 行转列（条件聚合）
来源：http://dnd.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cfd.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xgc.jinqigfzy.top

[Q89] 判断表是否存在
来源：http://vty.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://swx.zhengqikj.top

[Q90] 生成序号列
来源：http://cjx.yueranfly.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gkp.quarkkingdee.top

================================================================================
来源：http://nzu.chenzaomai.com

R. Bash 专题
来源：http://djz.jqgufenzy.top

================================================================================
来源：http://rtu.birdmap.top

[R01] shebang 与严格模式
来源：http://huj.havefunace.top

#!/usr/bin/env bash
来源：http://gap.hammf.cn

set -euo pipefail
来源：http://tsr.hysaishi.cn

[R02] 变量赋值与使用
来源：http://ydt.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://wjv.zhongyouzk.top

[R03] 只读变量
来源：http://vaw.daxiang520.top

readonly PI=3.14
来源：http://kxk.cucudq.cn

[R04] 位置参数
来源：http://pza.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kgt.mhx1999.top

[R05] 参数默认值
来源：http://suv.shanyushiyangkeji.top

name="${1:-default}"
来源：http://mno.hesvh.cn

[R06] 判断命令是否存在
来源：http://mgr.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lqc.jqgufenzy.top

[R07] if 判断文件
来源：http://rgn.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ejo.cqqwz.cn

[R08] 数值比较
来源：http://tan.iojbl.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tno.gaohongyu789.top

[R09] 字符串比较
来源：http://fbu.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cat.c1oappe.top

[R10] 正则匹配
来源：http://stu.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://efb.0kj1m.cn

[R11] case 多分支
来源：http://cay.tian-w.cn

case "$1" in
来源：http://xgc.hywenlv.cn

start) echo "启动" ;;
来源：http://kgq.0kj1m.cn

stop)  echo "停止" ;;
来源：http://idd.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://zlx.yongpay.top

esac
来源：http://xzm.wangshuangyany.cn

[R12] for 遍历文件
来源：http://psd.bjfxy.top

for f in *.txt; do echo "$f"; done
来源：http://igx.yonumen.top

[R13] for 计数循环
来源：http://iod.xuetiantiany.cn

for i in {1..10}; do echo "$i"; done
来源：http://bgi.jlsjyb.cn

[R14] C 风格 for
来源：http://oky.cucudq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vtu.jyoumei.cn

[R15] while 逐行读文件
来源：http://sty.aibaodan.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yun.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://hvm.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jdt.chenzaomai.com

[R17] 数组定义与取值
来源：http://qmv.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://yrd.tanke756.top

[R18] 遍历数组
来源：http://atn.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jqa.ybcxt.top

[R19] 数组长度
来源：http://pos.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://ljf.birdmap.top

[R20] 关联数组（字典）
来源：http://fkn.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gmi.ehwqpu.com

[R21] 字符串长度
来源：http://kis.gogol.net.cn

echo "${#s}"
来源：http://hyq.zhaomingkeji.xyz

[R22] 截取子串
来源：http://xem.ctjpmb.com

echo "${s:0:5}"
来源：http://ojy.hysaishi.cn

[R23] 字符串替换
来源：http://yos.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://asv.ybcxt.top

[R24] 大小写转换
来源：http://lpq.snrcjt.cn

echo "${s^^}"; echo "${s,,}"
来源：http://owv.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://tmn.ppjwa.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://stq.zdbjq.cn

[R26] 命令替换
来源：http://jnn.nanxuanxn.top

now=$(date +%F); echo "$now"
来源：http://kxe.hesvh.cn

[R27] 算术展开
来源：http://cqq.tian-w.cn

echo $((1 + 2 * 3))
来源：http://ygx.pycfn.com

[R28] 浮点运算
来源：http://kbb.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://krh.zhaomingkeji.xyz

[R29] 定义函数
来源：http://ywu.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cce.svipenyu.cn

[R30] 函数返回状态码
来源：http://hsm.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://uik.jqgufenzy.top

[R31] 局部变量
来源：http://tnv.mhx1999.top

f() { local x=1; echo "$x"; }
来源：http://wam.ctjpmb.com

[R32] 参数个数校验
来源：http://cvc.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kxo.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://qjl.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lug.vehdjk.com

[R34] 退出时清理
来源：http://dfm.feifeiyinyue.top

trap 'rm -f "$tmp"' EXIT
来源：http://clq.bjfxy.top

[R35] 后台执行并等待
来源：http://jnn.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://unx.fzhhl.top

[R36] 并发执行多个任务
来源：http://kgi.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tfl.daria6918.cn

[R37] 把输出赋给变量
来源：http://ium.aibaodan.cn

files=$(ls -1)
来源：http://bnc.hysaishi.cn

[R38] 管道串联
来源：http://zdg.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://gdg.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://hkv.dashuyun.cn

cmd > out.log 2>&1
来源：http://mst.guannengcc.top

[R40] 追加写日志
来源：http://owy.0kj1m.cn

echo "log" >> out.log
来源：http://lhp.feifeiyinyue.top

[R41] 丢弃输出
来源：http://osz.bbcook.cn

cmd >/dev/null 2>&1
来源：http://bkq.zhongyouzk.top

[R42] 输入重定向
来源：http://uuv.gzhubu.top

wc -l < a.txt
来源：http://vld.yj202588.top

[R43] 按名字查找文件
来源：http://blf.dianchejie.cn

find . -name "*.log" -type f
来源：http://wna.zycfv.cn

[R44] 按修改时间查找
来源：http://teq.zhoulong.xyz

find . -mtime -7 -type f
来源：http://ysl.nwbrower.top

[R45] 批量删除
来源：http://hbw.uphjek.com

find . -name "*.tmp" -delete
来源：http://zfw.bjfxy.top

[R46] 递归替换文件内容
来源：http://ciy.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nqi.jinqigufen.top

[R47] sed 单行替换
来源：http://had.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://xne.yuxming.cn

[R48] awk 取指定列
来源：http://ngv.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://tvg.zdbjq.cn

[R49] awk 带条件
来源：http://prd.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ftz.dianchejie.cn

[R50] awk 求和
来源：http://zzv.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://xgk.sjlbkw.cn

[R51] 排序去重取前几
来源：http://agy.pengpengdd.cyou

sort a.txt | uniq -c | sort -rn | head
来源：http://zub.dianchejie.cn

[R52] 统计行数
来源：http://tmo.iojbl.cn

wc -l a.txt
来源：http://hfn.uphjek.com

[R53] 查看文件头与实时尾
来源：http://kbb.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://poj.sufxvd.cn

[R54] 比较两个文件
来源：http://xvc.jyoumei.cn

diff a.txt b.txt
来源：http://tla.redwolf501.top

[R55] 压缩与解压
来源：http://gbw.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dhh.gzhubu.top

[R56] 远程拷贝
来源：http://wyv.tianlin.xyz

scp file user@host:/path/
来源：http://yzx.jianghu66.top

[R57] 远程执行命令
来源：http://phw.yangfankeji.com

ssh user@host 'uptime'
来源：http://uvy.guowangkeji.top

[R58] 下载文件
来源：http://eat.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kgm.yonumen.top

[R59] 发 POST JSON
来源：http://iqa.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sgl.gogol.net.cn

[R60] 只看 HTTP 状态码
来源：http://eqo.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ftc.havefunace.top

[R61] 磁盘占用
来源：http://clm.gaohongyu789.top

df -h;  du -sh *
来源：http://glj.dianchejie.cn

[R62] 找最占空间的文件
来源：http://glr.316326.xyz

du -ah . | sort -rh | head -10
来源：http://vwe.fktsv.cn

[R63] 内存与进程
来源：http://kiq.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://cgi.tarul.cn

[R64] 结束进程
来源：http://fsg.havefunace.top

kill -9 $(pgrep -f app.py)
来源：http://piz.yonumen.top

[R65] 查看端口占用
来源：http://wib.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bmm.hnqzz.top

[R66] 定时任务
来源：http://qct.cdnleiting.top

crontab -e;  crontab -l
来源：http://xdu.gzhubu.top

[R67] 生成随机十六进制串
来源：http://gqp.shangyingyoupin.top

openssl rand -hex 16
来源：http://qkt.andypj.xyz

[R68] 计算文件校验值
来源：http://qcl.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://acw.jiagoushi.top

[R69] 生成随机密码
来源：http://knn.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://znh.guannengcc.top

[R70] 时间戳与互转
来源：http://jqg.yuanzhike.top

date +%s;  date -d @1700000000
来源：http://ehr.sjlbkw.cn

[R71] 日期格式化
来源：http://drs.yj202588.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mgb.kuanghao11.cn

[R72] 等待端口就绪
来源：http://sjv.meibo888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://crf.chenjidiqi.icu

[R73] 分割大日志
来源：http://ggx.hesvh.cn

split -l 1000 big.log part_
来源：http://fdv.hywenlv.cn

[R74] 批量重命名
来源：http://acg.ppjwa.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ejv.jqgufenzy.top

[R75] 导出环境变量
来源：http://wsg.jqgufenzy.top

export PATH="$HOME/bin:$PATH"
来源：http://ywe.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://ndq.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://suv.yangfankeji.com

[R77] 读取用户输入
来源：http://ubb.yanxiufei.cn

read -rp "请输入: " ans
来源：http://ilp.fanxiaobao.xyz

[R78] 交互式菜单
来源：http://yyc.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hof.yfazqb.com

[R79] 解析命令行选项
来源：http://lvv.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yff.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://wuj.yj20258888.top

time ./run.sh
来源：http://foh.fanxiaobao.xyz

================================================================================
来源：http://osb.zhongyouzk.top

S. C / C++ 专题
来源：http://qna.jinqigfzy.top

================================================================================
来源：http://zen.9152youxi.cn

[S01] C：Hello World
来源：http://rgf.tianlin.xyz

#include <stdio.h>
来源：http://xbd.mhx1999.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://myl.jqgufenzy.top

[S02] C：变量与格式化输出
来源：http://qiz.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://eid.gaohongyu789.top

[S03] C：读入整数
来源：http://cmm.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://jeh.feifeiyinyue.top

[S04] C：字符串复制
来源：http://urx.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://ubp.snrcjt.cn

[S05] C：字符串长度
来源：http://bct.jlsjyb.cn

strlen(s)
来源：http://tjr.hnqzz.top

[S06] C：字符串比较
来源：http://ava.c1oappe.top

strcmp(a, b) == 0
来源：http://srw.yfazqb.com

[S07] C：数组遍历求和
来源：http://aso.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lou.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://rpu.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zuz.yvedp.cn

[S09] C：结构体定义与初始化
来源：http://uyb.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mcb.jqgfzy.top

[S10] C：指针与解引用
来源：http://nyj.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://nvb.kuanghao11.cn

[S11] C：逐行读文件
来源：http://ivi.zhengqikj.top


<!-- 参考信息 -->