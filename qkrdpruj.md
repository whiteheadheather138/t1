代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yda.hongshengwenyu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zwr.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cdv.nwbrower.top

[Q41] 多表连接
来源：http://iwv.yj20258888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://omo.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://uup.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://cen.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://eno.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://duk.cashguo.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xvx.ywan-chungtsiang.top

[Q43] 标量子查询
来源：http://ypo.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uyk.cdnleiting.top

[Q44] IN 子查询
来源：http://xdx.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oyp.ehwqpu.com

[Q45] EXISTS 判断存在
来源：http://cud.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wko.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://xmz.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://osr.gzhubu.top

[Q47] 与平均值比较
来源：http://mqv.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tvz.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://qhj.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ydj.0kj1m.cn

SELECT * FROM t WHERE c > 5;
来源：http://wnv.zycfv.cn

[Q49] 更新单行
来源：http://aqq.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oqz.uphjek.com

[Q50] 批量更新
来源：http://gpk.xylfe.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yvl.kuanghao11.cn

[Q51] 用子查询更新
来源：http://gom.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gll.chenzaomai.com

[Q52] 删除指定行
来源：http://fyj.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://ann.zhengqikj.top

[Q53] 按条件删除
来源：http://isq.dianchejie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cql.sweek.top

[Q54] 清空表
来源：http://ceg.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://khp.hfpthk.cn

[Q55] 排名（并列占位）
来源：http://pir.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nkx.jinqigufen.top

[Q56] 密集排名（并列不占位）
来源：http://veq.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pdg.fengsongda.top

[Q57] 行号
来源：http://zmu.uphjek.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wty.nanxuanxn.top

[Q58] 累计求和
来源：http://esh.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://khp.jlsjyb.cn

[Q59] 分组内累计
来源：http://ppz.xuetiantiany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gwk.daxiang520.top

[Q60] 取上一行 / 下一行
来源：http://xly.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jev.snrcjt.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uux.birdmap.top

[Q61] 移动平均
来源：http://oyj.redwolf501.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mrx.sjlbkw.cn

[Q62] 分组占比
来源：http://jzc.xuanzx.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ouf.quarkkingdee.top

[Q63] 开启事务
来源：http://bci.yueranfly.top

START TRANSACTION;                -- 或 BEGIN
来源：http://iym.hcnkem.com

[Q64] 提交事务
来源：http://fim.shangyingyoupin.top

COMMIT;
来源：http://cxh.guowangkeji.top

[Q65] 回滚事务
来源：http://nxa.hfpthk.cn

ROLLBACK;
来源：http://mxt.shanyushiyangkeji.top

[Q66] 行锁查询
来源：http://qia.cashguo.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gwe.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://ucv.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jkj.ehwqpu.com

[Q68] 保存点
来源：http://lhc.hcnkem.com

SAVEPOINT sp1;
来源：http://yuc.cucudq.cn

ROLLBACK TO sp1;
来源：http://dzm.vqdsnc.cn

[Q69] 查看执行计划
来源：http://yan.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ihq.jiagoushi.top

[Q70] 更新统计信息
来源：http://uds.ydjk.org.cn

ANALYZE TABLE users;
来源：http://voi.guannengcc.top

[Q71] 查看建表语句
来源：http://uvb.iojbl.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tiu.bjfxy.top

[Q72] 查看索引
来源：http://cdw.jinqigufen.top

SHOW INDEX FROM users;
来源：http://lfj.ivvv.top

[Q73] 查看表状态
来源：http://gil.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dny.xuetiantiany.cn

[Q74] 强制使用索引
来源：http://web.ppjwa.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bqd.shangyingyoupin.top

[Q75] 日期格式化
来源：http://ypp.cashguo.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mqf.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zpz.jlsjyb.cn

[Q76] 按天统计
来源：http://oea.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://srs.andypj.xyz

[Q77] 时间加减
来源：http://tza.zdqjudy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rjc.hnqzz.top

[Q78] 当前时间
来源：http://uwf.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uhd.yanxiufei.cn

[Q79] 字符串拼接
来源：http://jiz.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://spp.shangyingyoupin.top

[Q80] 字符串截取
来源：http://xnm.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ign.bbcook.cn

[Q81] 字符串替换
来源：http://vmz.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sgh.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://yfj.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xos.yongpay.top

[Q83] 大小写转换
来源：http://rjq.chenjidiqi.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://por.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://xxe.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://cvl.yangfankeji.com

[Q85] 数值取整
来源：http://fuc.jqgufenzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rte.daxiang520.top

[Q86] 读取 JSON 字段
来源：http://bvs.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ttd.cheryme.top

[Q87] JSON 字段做条件
来源：http://ldu.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qcy.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://odb.yongpay.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wrk.zhixingplan.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://biy.yvedp.cn

[Q89] 判断表是否存在
来源：http://voj.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tmp.dashuyun.cn

[Q90] 生成序号列
来源：http://yeb.shanyushiyangtech.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mep.hywenlv.cn

================================================================================
来源：http://rvp.9152youxi.cn

R. Bash 专题
来源：http://aoe.quarkkingdee.top

================================================================================
来源：http://ndt.tarul.cn

[R01] shebang 与严格模式
来源：http://gdn.sweek.top

#!/usr/bin/env bash
来源：http://ael.snrcjt.cn

set -euo pipefail
来源：http://ybe.yj20258.top

[R02] 变量赋值与使用
来源：http://aog.yuanzhike.top

name="Tom"; echo "$name"
来源：http://trw.epnwcf.com

[R03] 只读变量
来源：http://xag.birdmap.top

readonly PI=3.14
来源：http://rlb.xuanzx.com

[R04] 位置参数
来源：http://grl.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cvg.ppjwa.cn

[R05] 参数默认值
来源：http://lec.bjfxy.top

name="${1:-default}"
来源：http://bhd.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://wpx.jinqigfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tgu.redwolf501.top

[R07] if 判断文件
来源：http://xsn.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mqu.cheryme.top

[R08] 数值比较
来源：http://gjq.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://cfy.fanxiaobao.xyz

[R09] 字符串比较
来源：http://ekm.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qrn.0kj1m.cn

[R10] 正则匹配
来源：http://uco.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://onp.ivvv.top

[R11] case 多分支
来源：http://bhw.hywenlv.cn

case "$1" in
来源：http://ybo.zhoulong.xyz

start) echo "启动" ;;
来源：http://vsx.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://dog.xziqi.cn

*)     echo "未知命令" ;;
来源：http://wnl.andypj.xyz

esac
来源：http://xvx.gzhubu.top

[R12] for 遍历文件
来源：http://khl.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://xpx.gzhubu.top

[R13] for 计数循环
来源：http://qns.meibo888.top

for i in {1..10}; do echo "$i"; done
来源：http://oho.hongshengwenyu.top

[R14] C 风格 for
来源：http://gbb.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wly.haohaochexian.top

[R15] while 逐行读文件
来源：http://ecq.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ivm.jinqigufen.top

[R16] until 等待条件
来源：http://tpp.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mhj.jianghu66.top

[R17] 数组定义与取值
来源：http://nvd.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://iiz.feifeiyinyue.top

[R18] 遍历数组
来源：http://dap.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gwq.cqqwz.cn

[R19] 数组长度
来源：http://xyl.jinghuilouyu.cn

echo "${#arr[@]}"
来源：http://nzp.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://fpa.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lvl.tianlin.xyz

[R21] 字符串长度
来源：http://lom.yvedp.cn

echo "${#s}"
来源：http://iiv.kuanghao11.cn

[R22] 截取子串
来源：http://xfo.uphjek.com

echo "${s:0:5}"
来源：http://xhp.smart0.xyz

[R23] 字符串替换
来源：http://ncb.dashuyun.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wad.yonumen.top

[R24] 大小写转换
来源：http://mqs.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://yfs.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://uyi.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rtn.guowangkeji.top

[R26] 命令替换
来源：http://wcs.ydzc1.top

now=$(date +%F); echo "$now"
来源：http://bff.xziqi.cn

[R27] 算术展开
来源：http://jqg.hcnkem.com

echo $((1 + 2 * 3))
来源：http://sit.iojbl.cn

[R28] 浮点运算
来源：http://nqt.chenlongwang.top

echo "scale=2; 10/3" | bc
来源：http://qip.zhoulong.xyz

[R29] 定义函数
来源：http://dqb.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ooo.havefunace.top

[R30] 函数返回状态码
来源：http://oci.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://mex.jinqigufen.top

[R31] 局部变量
来源：http://pen.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://cxa.wangdashe.top

[R32] 参数个数校验
来源：http://fgd.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ebr.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://opr.epnwcf.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rvp.hnqzz.top

[R34] 退出时清理
来源：http://znq.yonumen.top

trap 'rm -f "$tmp"' EXIT
来源：http://qpb.jqgfzy.top

[R35] 后台执行并等待
来源：http://oib.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://gpc.yvedp.cn

[R36] 并发执行多个任务
来源：http://siq.yuanzhike.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vnx.wangdashe.top

[R37] 把输出赋给变量
来源：http://dzj.pycfn.com

files=$(ls -1)
来源：http://dfg.chenjidiqi.icu

[R38] 管道串联
来源：http://ufl.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://lsn.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://ncf.jianghu66.top

cmd > out.log 2>&1
来源：http://gvh.birdmap.top

[R40] 追加写日志
来源：http://bez.hammf.cn

echo "log" >> out.log
来源：http://dsb.yonumen.top

[R41] 丢弃输出
来源：http://uhy.meibo888.top

cmd >/dev/null 2>&1
来源：http://qrg.fengsongda.top

[R42] 输入重定向
来源：http://ohs.xziqi.cn

wc -l < a.txt
来源：http://wta.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://iun.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://but.haohaochexian.top

[R44] 按修改时间查找
来源：http://pxy.xziqi.cn

find . -mtime -7 -type f
来源：http://ubm.jinqigfzy.top

[R45] 批量删除
来源：http://yzq.9152youxi.cn

find . -name "*.tmp" -delete
来源：http://xei.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://abr.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pgd.hcnkem.com

[R47] sed 单行替换
来源：http://yuh.wangdashe.top

sed -i 's/foo/bar/g' a.txt
来源：http://wjp.chenjidiqi.icu

[R48] awk 取指定列
来源：http://xzh.hammf.cn

awk '{print $1, $3}' a.txt
来源：http://eyc.zhixingplan.top

[R49] awk 带条件
来源：http://mcq.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ben.havefunace.top

[R50] awk 求和
来源：http://rex.hongshengwenyu.top

awk '{s += $2} END {print s}' a.txt
来源：http://akz.birdmap.top

[R51] 排序去重取前几
来源：http://nme.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://mtd.aizwys.cn

[R52] 统计行数
来源：http://bwz.xingfuxueyuan.xyz

wc -l a.txt
来源：http://epp.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://erg.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dbw.shuidangran.top

[R54] 比较两个文件
来源：http://vym.vehdjk.com

diff a.txt b.txt
来源：http://gfd.jlsjyb.cn

[R55] 压缩与解压
来源：http://hso.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ysi.ywan-chungtsiang.top

[R56] 远程拷贝
来源：http://nff.redwolf501.top

scp file user@host:/path/
来源：http://she.ydzc1.top

[R57] 远程执行命令
来源：http://cqv.chenlongwang.top

ssh user@host 'uptime'
来源：http://raz.andypj.xyz

[R58] 下载文件
来源：http://kmv.shanyushiyangtech.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dve.9152youxi.cn

[R59] 发 POST JSON
来源：http://cmw.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kzj.kuanghao11.cn

[R60] 只看 HTTP 状态码
来源：http://kko.guowangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vyc.tanke756.top

[R61] 磁盘占用
来源：http://evo.ppjwa.cn

df -h;  du -sh *
来源：http://xru.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://bjs.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://djv.tarul.cn

[R63] 内存与进程
来源：http://rqp.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://pwn.ivvv.top

[R64] 结束进程
来源：http://aer.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://cic.hywenlv.cn

[R65] 查看端口占用
来源：http://aqo.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ikz.tarul.cn

[R66] 定时任务
来源：http://zvx.havefunace.top

crontab -e;  crontab -l
来源：http://pvh.fehbvm.com

[R67] 生成随机十六进制串
来源：http://ivd.uphjek.com

openssl rand -hex 16
来源：http://evs.sjlbkw.cn

[R68] 计算文件校验值
来源：http://mxt.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xuu.daxiang520.top

[R69] 生成随机密码
来源：http://jri.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://zya.bbcook.cn

[R70] 时间戳与互转
来源：http://tmp.tian-w.cn

date +%s;  date -d @1700000000
来源：http://coy.jyoumei.cn

[R71] 日期格式化
来源：http://olj.0kj1m.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://orr.jiagoushi.top

[R72] 等待端口就绪
来源：http://rwx.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://qfg.ppjwa.cn

[R73] 分割大日志
来源：http://roz.iojbl.cn

split -l 1000 big.log part_
来源：http://ays.yangfankeji.com

[R74] 批量重命名
来源：http://oab.daxiang520.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wev.yangfankeji.com

[R75] 导出环境变量
来源：http://utc.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://ytc.chenjidiqi.icu

[R76] 使用临时文件
来源：http://ied.kuanghao11.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mrt.tian-w.cn

[R77] 读取用户输入
来源：http://dvm.cucudq.cn

read -rp "请输入: " ans
来源：http://sna.shangyingyoupin.top

[R78] 交互式菜单
来源：http://fxg.shzxlz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://joa.dianchejie.cn

[R79] 解析命令行选项
来源：http://ylj.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vdj.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://lly.feifeiyinyue.top

time ./run.sh
来源：http://vvl.guannengcc.top

================================================================================
来源：http://vcc.zhoulong.xyz

S. C / C++ 专题
来源：http://vyc.zhengqikj.top

================================================================================
来源：http://wds.tarul.cn

[S01] C：Hello World
来源：http://aok.jqgfzy.top

#include <stdio.h>
来源：http://cwv.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://msu.xinyue.icu

[S02] C：变量与格式化输出
来源：http://bll.yuxming.cn

int a = 10; printf("%d\n", a);
来源：http://usc.iojbl.cn

[S03] C：读入整数
来源：http://rhh.xinyue.icu

int x; scanf("%d", &x);
来源：http://tsq.shangyingyoupin.top

[S04] C：字符串复制
来源：http://njo.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yhr.zhongyouzk.top

[S05] C：字符串长度
来源：http://ues.jyoumei.cn

strlen(s)
来源：http://qen.feifeiyinyue.top

[S06] C：字符串比较
来源：http://aiw.yuanzhike.top

strcmp(a, b) == 0
来源：http://net.hysaishi.cn

[S07] C：数组遍历求和
来源：http://zlj.wangshuangyany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tad.birdmap.top

[S08] C：动态内存分配与释放
来源：http://kup.zdqjudy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hse.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://aji.fanxiaobao.xyz


<!-- 参考信息 -->