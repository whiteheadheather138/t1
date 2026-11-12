代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://xjs.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://phh.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://ltj.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://uhq.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://cdy.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hyg.cucudq.cn

[Q43] 标量子查询
来源：http://ggo.feifeiyinyue.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rkk.yuxming.cn

[Q44] IN 子查询
来源：http://bsw.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lsu.wangshuangyany.cn

[Q45] EXISTS 判断存在
来源：http://qbw.zhaomingkeji.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sad.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ndt.vehdjk.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fiv.jinqigfzy.top

[Q47] 与平均值比较
来源：http://yvi.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yuh.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://ynr.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kml.gogol.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://eqe.yj20258.top

[Q49] 更新单行
来源：http://yqa.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uqw.bbcook.cn

[Q50] 批量更新
来源：http://ane.yj20258.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ado.dianchejie.cn

[Q51] 用子查询更新
来源：http://cfu.yangfankeji.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jzh.xinyue.icu

[Q52] 删除指定行
来源：http://plt.jianghu66.top

DELETE FROM users WHERE id = 10;
来源：http://vqo.cdnleiting.top

[Q53] 按条件删除
来源：http://fws.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qxs.jinqigfzy.top

[Q54] 清空表
来源：http://gla.gzhubu.top

TRUNCATE TABLE logs;
来源：http://yte.yj20258888.top

[Q55] 排名（并列占位）
来源：http://cti.dianchejie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zmz.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://dnm.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mzs.daria6918.cn

[Q57] 行号
来源：http://kxl.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nho.gogol.net.cn

[Q58] 累计求和
来源：http://ebe.guowangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://run.nanxinkj.top

[Q59] 分组内累计
来源：http://psi.yvedp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jmg.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://tok.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bar.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zki.gzhubu.top

[Q61] 移动平均
来源：http://kjb.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qiz.tianlin.xyz

[Q62] 分组占比
来源：http://hng.dianchejie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lws.fzhhl.top

[Q63] 开启事务
来源：http://qtl.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mnr.cqqwz.cn

[Q64] 提交事务
来源：http://qdp.shuidangran.top

COMMIT;
来源：http://xxx.zhiwuduotai.top

[Q65] 回滚事务
来源：http://xji.sweek.top

ROLLBACK;
来源：http://vaw.9152youxi.cn

[Q66] 行锁查询
来源：http://ear.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dip.fzhhl.top

[Q67] 设置隔离级别
来源：http://opb.aizwys.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dfp.vqdsnc.cn

[Q68] 保存点
来源：http://tzy.ydzc1.top

SAVEPOINT sp1;
来源：http://inu.shanyushiyangtech.top

ROLLBACK TO sp1;
来源：http://hcd.xinyue.icu

[Q69] 查看执行计划
来源：http://xvq.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kqq.jyoumei.cn

[Q70] 更新统计信息
来源：http://fhk.52xcode.cn

ANALYZE TABLE users;
来源：http://pwi.yj202588.top

[Q71] 查看建表语句
来源：http://gsu.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tub.dianchejie.cn

[Q72] 查看索引
来源：http://dsl.fehbvm.com

SHOW INDEX FROM users;
来源：http://oni.cucudq.cn

[Q73] 查看表状态
来源：http://iou.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ynz.tian-w.cn

[Q74] 强制使用索引
来源：http://rcv.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kdv.hywenlv.cn

[Q75] 日期格式化
来源：http://ybe.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rmf.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bvz.9152youxi.cn

[Q76] 按天统计
来源：http://rlc.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wti.guowangkeji.top

[Q77] 时间加减
来源：http://zly.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uzo.ydjk.org.cn

[Q78] 当前时间
来源：http://wik.dianchejie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ycj.uphjek.com

[Q79] 字符串拼接
来源：http://aqm.andypj.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wzp.0kj1m.cn

[Q80] 字符串截取
来源：http://ije.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hui.ivvv.top

[Q81] 字符串替换
来源：http://vwq.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cuv.tarul.cn

[Q82] 字符长度与字节长度
来源：http://iak.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qci.guannengcc.top

[Q83] 大小写转换
来源：http://ewo.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lvt.guowangkeji.top

[Q84] 去除首尾空格
来源：http://kej.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://dsw.gogol.net.cn

[Q85] 数值取整
来源：http://oze.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aih.andypj.xyz

[Q86] 读取 JSON 字段
来源：http://zjt.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jqn.52xcode.cn

[Q87] JSON 字段做条件
来源：http://qdh.xuetiantiany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://est.feifeiyinyue.top

[Q88] 行转列（条件聚合）
来源：http://zxn.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jrt.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gwi.ybcxt.top

[Q89] 判断表是否存在
来源：http://dhh.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ecs.dashuyun.cn

[Q90] 生成序号列
来源：http://zso.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gwl.nanxuanxn.top

================================================================================
来源：http://sqf.ydzc1.top

R. Bash 专题
来源：http://dnn.yonumen.top

================================================================================
来源：http://apy.ehwqpu.com

[R01] shebang 与严格模式
来源：http://sdl.xuanzx.com

#!/usr/bin/env bash
来源：http://srz.jlsjyb.cn

set -euo pipefail
来源：http://dab.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://pjj.vehdjk.com

name="Tom"; echo "$name"
来源：http://ggv.jiagoushi.top

[R03] 只读变量
来源：http://aau.cashguo.top

readonly PI=3.14
来源：http://aea.vehdjk.com

[R04] 位置参数
来源：http://mlh.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://psh.haohaochexian.top

[R05] 参数默认值
来源：http://iqy.zhiwuduotai.top

name="${1:-default}"
来源：http://rof.jianghu66.top

[R06] 判断命令是否存在
来源：http://pfs.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qmf.mhx1999.top

[R07] if 判断文件
来源：http://psm.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dvb.daria6918.cn

[R08] 数值比较
来源：http://snr.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cye.fktsv.cn

[R09] 字符串比较
来源：http://mvu.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yyw.zhongyouzk.top

[R10] 正则匹配
来源：http://xib.jiagoushi.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mjb.quarkkingdee.top

[R11] case 多分支
来源：http://lue.mhx1999.top

case "$1" in
来源：http://ose.xinyue.icu

start) echo "启动" ;;
来源：http://wds.cdnleiting.top

stop)  echo "停止" ;;
来源：http://pgj.cheryme.top

*)     echo "未知命令" ;;
来源：http://lyf.gaohongyu789.top

esac
来源：http://xvn.snrcjt.cn

[R12] for 遍历文件
来源：http://frm.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://nnw.mhx1999.top

[R13] for 计数循环
来源：http://nvw.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://xge.hywenlv.cn

[R14] C 风格 for
来源：http://zxn.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eml.cqqwz.cn

[R15] while 逐行读文件
来源：http://atp.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://alg.aibaodan.cn

[R16] until 等待条件
来源：http://qzp.cheryme.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jkz.yvedp.cn

[R17] 数组定义与取值
来源：http://oni.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mav.zhoulong.xyz

[R18] 遍历数组
来源：http://dyn.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vwd.pengpengdd.cyou

[R19] 数组长度
来源：http://irt.aizwys.cn

echo "${#arr[@]}"
来源：http://drm.shanyushiyangtech.top

[R20] 关联数组（字典）
来源：http://lkc.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jgx.kuanghao11.cn

[R21] 字符串长度
来源：http://jmb.cashguo.top

echo "${#s}"
来源：http://vxv.ctjpmb.com

[R22] 截取子串
来源：http://sqz.jlsjyb.cn

echo "${s:0:5}"
来源：http://vaq.shzxlz.cn

[R23] 字符串替换
来源：http://lrs.ybcxt.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uda.yueranfly.top

[R24] 大小写转换
来源：http://vto.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://sfv.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://bls.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://xpd.zdqjudy.top

[R26] 命令替换
来源：http://gyk.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://fjt.fanxiaobao.xyz

[R27] 算术展开
来源：http://ddp.sjlbkw.cn

echo $((1 + 2 * 3))
来源：http://cih.xziqi.cn

[R28] 浮点运算
来源：http://jra.hnxiangtu.top

echo "scale=2; 10/3" | bc
来源：http://dtb.tarul.cn

[R29] 定义函数
来源：http://vxx.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://spn.yvedp.cn

[R30] 函数返回状态码
来源：http://ifm.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://nta.cucudq.cn

[R31] 局部变量
来源：http://xym.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://cuu.jinqigfzy.top

[R32] 参数个数校验
来源：http://lwx.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sdf.cheryme.top

[R33] 捕获错误并提示行号
来源：http://exf.yj20258888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rym.quarkkingdee.top

[R34] 退出时清理
来源：http://jyi.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://wjs.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://xon.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://gsw.hammf.cn

[R36] 并发执行多个任务
来源：http://lgr.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ehb.xylfe.cn

[R37] 把输出赋给变量
来源：http://gbg.jyoumei.cn

files=$(ls -1)
来源：http://owp.fzhhl.top

[R38] 管道串联
来源：http://jva.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://evx.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://nok.cdnleiting.top

cmd > out.log 2>&1
来源：http://qsn.sweek.top

[R40] 追加写日志
来源：http://unx.ctjpmb.com

echo "log" >> out.log
来源：http://ngf.svipenyu.cn

[R41] 丢弃输出
来源：http://ela.guannengcc.top

cmd >/dev/null 2>&1
来源：http://pdi.smart0.xyz

[R42] 输入重定向
来源：http://eke.dashuyun.cn

wc -l < a.txt
来源：http://dnj.fktsv.cn

[R43] 按名字查找文件
来源：http://kgs.cashguo.top

find . -name "*.log" -type f
来源：http://mld.kuanghao11.cn

[R44] 按修改时间查找
来源：http://cjb.sweek.top

find . -mtime -7 -type f
来源：http://mfa.gzhubu.top

[R45] 批量删除
来源：http://dgh.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://uhy.andypj.xyz

[R46] 递归替换文件内容
来源：http://aes.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://frw.smart0.xyz

[R47] sed 单行替换
来源：http://wiy.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://aag.ydzc1.top

[R48] awk 取指定列
来源：http://zrz.gaohongyu789.top

awk '{print $1, $3}' a.txt
来源：http://rgz.birdmap.top

[R49] awk 带条件
来源：http://isk.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kro.yuanzhike.top

[R50] awk 求和
来源：http://rhz.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zco.nanxinkj.top

[R51] 排序去重取前几
来源：http://tav.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sed.ybcxt.top

[R52] 统计行数
来源：http://ijg.meibo888.top

wc -l a.txt
来源：http://mhf.fzhhl.top

[R53] 查看文件头与实时尾
来源：http://czx.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yhh.hysaishi.cn

[R54] 比较两个文件
来源：http://jrw.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://hcg.pengpengdd.cyou

[R55] 压缩与解压
来源：http://tnz.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wvr.sufxvd.cn

[R56] 远程拷贝
来源：http://zmj.sweek.top

scp file user@host:/path/
来源：http://qsz.andypj.xyz

[R57] 远程执行命令
来源：http://bqm.wangshuangyany.cn

ssh user@host 'uptime'
来源：http://suv.birdmap.top

[R58] 下载文件
来源：http://qnq.zhiwuduotai.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://stq.xuanzx.com

[R59] 发 POST JSON
来源：http://ymd.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hhb.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://zgi.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tqd.yuxming.cn

[R61] 磁盘占用
来源：http://jbp.ydzc1.top

df -h;  du -sh *
来源：http://ieh.tanke756.top

[R62] 找最占空间的文件
来源：http://drh.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://psb.kuanghao11.cn

[R63] 内存与进程
来源：http://djb.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://znc.zhijiandao.cn

[R64] 结束进程
来源：http://yaa.ppjwa.cn

kill -9 $(pgrep -f app.py)
来源：http://bjg.fehbvm.com

[R65] 查看端口占用
来源：http://fuu.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rul.yongpay.top

[R66] 定时任务
来源：http://clj.ppjwa.cn

crontab -e;  crontab -l
来源：http://twt.aizwys.cn

[R67] 生成随机十六进制串
来源：http://dss.hnxiangtu.top

openssl rand -hex 16
来源：http://mjq.jyoumei.cn

[R68] 计算文件校验值
来源：http://sqt.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://czv.vehdjk.com

[R69] 生成随机密码
来源：http://utf.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://giw.birdmap.top

[R70] 时间戳与互转
来源：http://fkj.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://rji.hnxiangtu.top

[R71] 日期格式化
来源：http://ytg.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://biz.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://mpr.birdmap.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lxj.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://dtg.ctjpmb.com

split -l 1000 big.log part_
来源：http://syn.zhijiandao.cn

[R74] 批量重命名
来源：http://qdi.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://amg.pengpengdd.cyou

[R75] 导出环境变量
来源：http://ryq.uphjek.com

export PATH="$HOME/bin:$PATH"
来源：http://lvu.yuanzhike.top

[R76] 使用临时文件
来源：http://wkz.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ard.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://eld.birdmap.top

read -rp "请输入: " ans
来源：http://lyx.iojbl.cn

[R78] 交互式菜单
来源：http://yhp.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jkt.jinqigufen.top

[R79] 解析命令行选项
来源：http://rzl.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vco.316326.xyz

[R80] 查看脚本执行耗时
来源：http://txd.bjfxy.top

time ./run.sh
来源：http://qge.zhixingplan.top

================================================================================
来源：http://wuz.sufxvd.cn

S. C / C++ 专题
来源：http://nnk.xinyue.icu

================================================================================
来源：http://bhm.chenzaomai.com

[S01] C：Hello World
来源：http://miw.wangshuangyany.cn

#include <stdio.h>
来源：http://htd.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cft.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://mpe.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://tnb.guannengcc.top

[S03] C：读入整数
来源：http://adg.hywenlv.cn

int x; scanf("%d", &x);
来源：http://ilo.sysykeji.top

[S04] C：字符串复制
来源：http://vbb.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xug.yuanzhike.top

[S05] C：字符串长度
来源：http://ser.jinyuanbaomall.cn

strlen(s)
来源：http://iew.guannengcc.top

[S06] C：字符串比较
来源：http://grf.sysykeji.top

strcmp(a, b) == 0
来源：http://tcv.sufxvd.cn

[S07] C：数组遍历求和
来源：http://fzs.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lba.yvedp.cn

[S08] C：动态内存分配与释放
来源：http://rzk.hfpthk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zwp.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://zic.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rah.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://dlu.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://dof.zhengqikj.top

[S11] C：逐行读文件
来源：http://qip.chenjidiqi.icu


<!-- 参考信息 -->