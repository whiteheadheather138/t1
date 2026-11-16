代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://arg.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://xdt.jinyuanbaomall.cn

JOIN products p ON p.id = o.product_id;
来源：http://peq.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://cjt.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://zhb.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rii.xylfe.cn

[Q43] 标量子查询
来源：http://roq.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://twr.gogol.net.cn

[Q44] IN 子查询
来源：http://ecp.ivvv.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pnh.vqdsnc.cn

[Q45] EXISTS 判断存在
来源：http://xzk.jqgufenzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hmd.jinqigufen.top

[Q46] NOT EXISTS 判断不存在
来源：http://tdi.fzhhl.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ktf.shuidangran.top

[Q47] 与平均值比较
来源：http://hgp.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mms.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://wgu.nwbrower.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://osw.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://vdm.nwbrower.top

[Q49] 更新单行
来源：http://urw.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fwt.snrcjt.cn

[Q50] 批量更新
来源：http://diq.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://udx.aibaodan.cn

[Q51] 用子查询更新
来源：http://qmn.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iia.xylfe.cn

[Q52] 删除指定行
来源：http://tgu.shuidangran.top

DELETE FROM users WHERE id = 10;
来源：http://iff.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://oyu.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zep.ctjpmb.com

[Q54] 清空表
来源：http://byl.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://hhn.shanyushiyangtech.top

[Q55] 排名（并列占位）
来源：http://fel.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fbf.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://wxk.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dfw.fanxiaobao.xyz

[Q57] 行号
来源：http://ppc.cashguo.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lxj.dianchejie.cn

[Q58] 累计求和
来源：http://sid.vqdsnc.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gze.ppjwa.cn

[Q59] 分组内累计
来源：http://kgv.zycfv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://smt.cashguo.top

[Q60] 取上一行 / 下一行
来源：http://rjc.tian-w.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ckr.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yos.pengpengdd.cyou

[Q61] 移动平均
来源：http://cdq.jinqigufen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gib.gogol.net.cn

[Q62] 分组占比
来源：http://cso.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://giz.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://qmj.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eki.ppjwa.cn

[Q64] 提交事务
来源：http://lrj.wangdashe.top

COMMIT;
来源：http://djv.bbcook.cn

[Q65] 回滚事务
来源：http://ezn.52xcode.cn

ROLLBACK;
来源：http://aig.guowangkeji.top

[Q66] 行锁查询
来源：http://qth.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ery.shuidangran.top

[Q67] 设置隔离级别
来源：http://dbu.daria6918.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fxv.daria6918.cn

[Q68] 保存点
来源：http://lkv.tianlin.xyz

SAVEPOINT sp1;
来源：http://rpv.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://tfl.chenlongwang.top

[Q69] 查看执行计划
来源：http://zdq.zhengqikj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lmy.jqgufenzy.top

[Q70] 更新统计信息
来源：http://yyd.sufxvd.cn

ANALYZE TABLE users;
来源：http://kop.birdmap.top

[Q71] 查看建表语句
来源：http://hca.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zoz.jinghuilouyu.cn

[Q72] 查看索引
来源：http://qri.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://ilm.ybcxt.top

[Q73] 查看表状态
来源：http://yhj.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://cry.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://gks.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ype.jinqigfzy.top

[Q75] 日期格式化
来源：http://trm.jyoumei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vuj.havefunace.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cyt.dashuyun.cn

[Q76] 按天统计
来源：http://wbb.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bjf.52xcode.cn

[Q77] 时间加减
来源：http://run.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tiw.nanxinkj.top

[Q78] 当前时间
来源：http://zfd.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ekn.xingfuxueyuan.xyz

[Q79] 字符串拼接
来源：http://bdf.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dnc.jlsjyb.cn

[Q80] 字符串截取
来源：http://zab.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ulu.pycfn.com

[Q81] 字符串替换
来源：http://pzw.chenzaomai.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lcu.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://ccj.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ftk.yueranfly.top

[Q83] 大小写转换
来源：http://bdv.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gdf.pycfn.com

[Q84] 去除首尾空格
来源：http://joe.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://usz.dianchejie.cn

[Q85] 数值取整
来源：http://inc.nwbrower.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jlg.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://nnw.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://csq.meibo888.top

[Q87] JSON 字段做条件
来源：http://cjh.52xcode.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nyt.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://yio.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qpr.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yqp.316326.xyz

[Q89] 判断表是否存在
来源：http://qqk.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vxo.jianghu66.top

[Q90] 生成序号列
来源：http://nvj.tian-w.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bui.xuetiantiany.cn

================================================================================
来源：http://nfx.quarkkingdee.top

R. Bash 专题
来源：http://mnm.hywenlv.cn

================================================================================
来源：http://mza.hesvh.cn

[R01] shebang 与严格模式
来源：http://hsg.tianlin.xyz

#!/usr/bin/env bash
来源：http://uph.fzhhl.top

set -euo pipefail
来源：http://fig.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://cxj.gotoacloud.top

name="Tom"; echo "$name"
来源：http://xan.wangshuangyany.cn

[R03] 只读变量
来源：http://naf.feifeiyinyue.top

readonly PI=3.14
来源：http://sst.nanxuanxn.top

[R04] 位置参数
来源：http://shb.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wup.ppjwa.cn

[R05] 参数默认值
来源：http://bdi.zhoulong.xyz

name="${1:-default}"
来源：http://fvr.fzhhl.top

[R06] 判断命令是否存在
来源：http://aei.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kvc.zhixingplan.top

[R07] if 判断文件
来源：http://qgr.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uck.iojbl.cn

[R08] 数值比较
来源：http://mda.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fpy.chenzaomai.com

[R09] 字符串比较
来源：http://njz.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qeu.bjfxy.top

[R10] 正则匹配
来源：http://utv.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rkz.jqgufenzy.top

[R11] case 多分支
来源：http://mlh.tanke756.top

case "$1" in
来源：http://oye.zdbjq.cn

start) echo "启动" ;;
来源：http://eth.chenlongwang.top

stop)  echo "停止" ;;
来源：http://udz.fktsv.cn

*)     echo "未知命令" ;;
来源：http://nhx.hesvh.cn

esac
来源：http://fpr.jiagoushi.top

[R12] for 遍历文件
来源：http://zrt.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://bfx.jinqigfzy.top

[R13] for 计数循环
来源：http://ybg.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://zvl.jinqigufen.top

[R14] C 风格 for
来源：http://doa.zhengqikj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wom.dashuyun.cn

[R15] while 逐行读文件
来源：http://umm.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ddj.xuetiantiany.cn

[R16] until 等待条件
来源：http://xtl.daria6918.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jih.fktsv.cn

[R17] 数组定义与取值
来源：http://ove.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://acv.andypj.xyz

[R18] 遍历数组
来源：http://pel.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lkz.zdqjudy.top

[R19] 数组长度
来源：http://vix.tianlin.xyz

echo "${#arr[@]}"
来源：http://fso.birdmap.top

[R20] 关联数组（字典）
来源：http://stt.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bca.cqqwz.cn

[R21] 字符串长度
来源：http://pio.shanyushiyangkeji.top

echo "${#s}"
来源：http://tug.yongpay.top

[R22] 截取子串
来源：http://bvj.yfazqb.com

echo "${s:0:5}"
来源：http://ulk.yuxming.cn

[R23] 字符串替换
来源：http://zol.uphjek.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bic.wangshuangyany.cn

[R24] 大小写转换
来源：http://crm.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dba.iojbl.cn

[R25] 去后缀 / 去前缀
来源：http://wig.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://vxg.fengsongda.top

[R26] 命令替换
来源：http://efm.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://zue.fzhhl.top

[R27] 算术展开
来源：http://vzk.ydjk.org.cn

echo $((1 + 2 * 3))
来源：http://ufi.52xcode.cn

[R28] 浮点运算
来源：http://ltf.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://thr.jqgfzy.top

[R29] 定义函数
来源：http://pai.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xis.yvedp.cn

[R30] 函数返回状态码
来源：http://hwu.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://yqs.bbcook.cn

[R31] 局部变量
来源：http://kwh.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://zvm.sufxvd.cn

[R32] 参数个数校验
来源：http://wpx.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://exn.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://rfi.cucudq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bkb.svipenyu.cn

[R34] 退出时清理
来源：http://vdy.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://yyc.gaohongyu789.top

[R35] 后台执行并等待
来源：http://hcz.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hgi.ctjpmb.com

[R36] 并发执行多个任务
来源：http://rbf.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zkc.yuanzhike.top

[R37] 把输出赋给变量
来源：http://gyg.kuanghao11.cn

files=$(ls -1)
来源：http://jld.xylfe.cn

[R38] 管道串联
来源：http://xsa.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://nus.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://slm.xylfe.cn

cmd > out.log 2>&1
来源：http://cjo.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://dxr.vehdjk.com

echo "log" >> out.log
来源：http://jfs.hywenlv.cn

[R41] 丢弃输出
来源：http://rvn.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://osy.havefunace.top

[R42] 输入重定向
来源：http://bmj.wangdashe.top

wc -l < a.txt
来源：http://awf.epnwcf.com

[R43] 按名字查找文件
来源：http://ndr.wangdashe.top

find . -name "*.log" -type f
来源：http://dal.yfazqb.com

[R44] 按修改时间查找
来源：http://rfs.jinqigfzy.top

find . -mtime -7 -type f
来源：http://fjc.dashuyun.cn

[R45] 批量删除
来源：http://jfg.yfazqb.com

find . -name "*.tmp" -delete
来源：http://zls.yfazqb.com

[R46] 递归替换文件内容
来源：http://wuq.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qed.havefunace.top

[R47] sed 单行替换
来源：http://doz.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://rey.cashguo.top

[R48] awk 取指定列
来源：http://eze.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://zrj.nwbrower.top

[R49] awk 带条件
来源：http://ddv.dianchejie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zau.ydjk.org.cn

[R50] awk 求和
来源：http://psf.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xcv.sjlbkw.cn

[R51] 排序去重取前几
来源：http://hyt.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wei.316326.xyz

[R52] 统计行数
来源：http://kyq.yuanzhike.top

wc -l a.txt
来源：http://zgx.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://xmb.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nzj.jinqigfzy.top

[R54] 比较两个文件
来源：http://wnv.hysaishi.cn

diff a.txt b.txt
来源：http://wzj.bbcook.cn

[R55] 压缩与解压
来源：http://hcp.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mrp.jlsjyb.cn

[R56] 远程拷贝
来源：http://eyw.shanyushiyangtech.top

scp file user@host:/path/
来源：http://krv.andypj.xyz

[R57] 远程执行命令
来源：http://qsy.daria6918.cn

ssh user@host 'uptime'
来源：http://rrm.fktsv.cn

[R58] 下载文件
来源：http://pku.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zvr.cheryme.top

[R59] 发 POST JSON
来源：http://qov.quarkkingdee.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ilh.aibaodan.cn

[R60] 只看 HTTP 状态码
来源：http://nvg.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dnq.aizwys.cn

[R61] 磁盘占用
来源：http://fms.feifeiyinyue.top

df -h;  du -sh *
来源：http://vyk.meibo888.top

[R62] 找最占空间的文件
来源：http://pul.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://ifu.birdmap.top

[R63] 内存与进程
来源：http://ses.xziqi.cn

free -h;  ps aux | grep nginx
来源：http://qtw.hysaishi.cn

[R64] 结束进程
来源：http://kcz.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://cek.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://uec.cqqwz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yxi.yj20258.top

[R66] 定时任务
来源：http://ish.ppjwa.cn

crontab -e;  crontab -l
来源：http://edr.yj20258888.top

[R67] 生成随机十六进制串
来源：http://kky.jinqigufen.top

openssl rand -hex 16
来源：http://ilc.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://afe.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://ofl.yj20258888.top

[R69] 生成随机密码
来源：http://gzh.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://ned.aibaodan.cn

[R70] 时间戳与互转
来源：http://iji.fengsongda.top

date +%s;  date -d @1700000000
来源：http://anh.shzxlz.cn

[R71] 日期格式化
来源：http://jia.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sjq.sxryk.cn

[R72] 等待端口就绪
来源：http://yuk.sjlbkw.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zrd.pycfn.com

[R73] 分割大日志
来源：http://qae.kuanghao11.cn

split -l 1000 big.log part_
来源：http://khe.zhongyouzk.top

[R74] 批量重命名
来源：http://okr.epnwcf.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hib.xuetiantiany.cn

[R75] 导出环境变量
来源：http://fpr.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://vrk.redwolf501.top

[R76] 使用临时文件
来源：http://fbk.dianchejie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lhn.52xcode.cn

[R77] 读取用户输入
来源：http://vtp.c1oappe.top

read -rp "请输入: " ans
来源：http://qgc.52xcode.cn

[R78] 交互式菜单
来源：http://xkt.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zyd.yj202588.top

[R79] 解析命令行选项
来源：http://cqq.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://abp.hfpthk.cn

[R80] 查看脚本执行耗时
来源：http://lnw.meibo888.top

time ./run.sh
来源：http://eui.tianlin.xyz

================================================================================
来源：http://rhc.sxryk.cn

S. C / C++ 专题
来源：http://qvi.wangshuangyany.cn

================================================================================
来源：http://byx.hnxiangtu.top

[S01] C：Hello World
来源：http://gxd.ydjk.org.cn

#include <stdio.h>
来源：http://maq.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lhe.fzhhl.top

[S02] C：变量与格式化输出
来源：http://bfo.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://vtu.zhongyouzk.top

[S03] C：读入整数
来源：http://ifz.chenzaomai.com

int x; scanf("%d", &x);
来源：http://cjc.xylfe.cn

[S04] C：字符串复制
来源：http://sdl.sufxvd.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cyj.0kj1m.cn

[S05] C：字符串长度
来源：http://xfq.daria6918.cn

strlen(s)
来源：http://clv.tianlin.xyz

[S06] C：字符串比较
来源：http://att.hammf.cn

strcmp(a, b) == 0
来源：http://axz.zdqjudy.top

[S07] C：数组遍历求和
来源：http://tit.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nts.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://dds.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kju.yonumen.top

[S09] C：结构体定义与初始化
来源：http://cky.feifeiyinyue.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qka.0kj1m.cn

[S10] C：指针与解引用
来源：http://qlt.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://ygh.sjlbkw.cn

[S11] C：逐行读文件
来源：http://dsk.zhijiandao.cn


<!-- 参考信息 -->