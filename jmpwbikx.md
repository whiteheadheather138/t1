代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hfu.zhaomingkeji.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://tjp.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dpd.ydzc1.top

[Q41] 多表连接
来源：http://ahz.52xcode.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wvk.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://bbs.ivvv.top

JOIN products p ON p.id = o.product_id;
来源：http://aye.316326.xyz

[Q42] 连接条件附加过滤
来源：http://ats.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://pep.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vzp.zhiwuduotai.top

[Q43] 标量子查询
来源：http://inv.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yxj.jqgfzy.top

[Q44] IN 子查询
来源：http://vny.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mrm.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://dwa.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wqi.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lxs.smart0.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fby.gotoacloud.top

[Q47] 与平均值比较
来源：http://lxo.yj20258888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ask.iojbl.cn

[Q48] CTE 公用表表达式
来源：http://esz.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zcu.smart0.xyz

SELECT * FROM t WHERE c > 5;
来源：http://vgh.ppjwa.cn

[Q49] 更新单行
来源：http://gxz.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://swu.xylfe.cn

[Q50] 批量更新
来源：http://mfe.yj20258888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dmt.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://luj.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hwl.zdbjq.cn

[Q52] 删除指定行
来源：http://klo.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://abu.fanxiaobao.xyz

[Q53] 按条件删除
来源：http://mlk.yangfankeji.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ugl.ydjk.org.cn

[Q54] 清空表
来源：http://uex.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://yqk.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://dgn.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kti.316326.xyz

[Q56] 密集排名（并列不占位）
来源：http://kzd.daxiang520.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://run.gaohongyu789.top

[Q57] 行号
来源：http://pvv.jinqigufen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rhi.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://kur.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jmb.tianlin.xyz

[Q59] 分组内累计
来源：http://jcw.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cta.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://ywt.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zlb.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kbu.hongshengwenyu.top

[Q61] 移动平均
来源：http://ksr.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lov.fzhhl.top

[Q62] 分组占比
来源：http://nhz.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iyf.hysaishi.cn

[Q63] 开启事务
来源：http://eok.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kij.dashuyun.cn

[Q64] 提交事务
来源：http://gzr.sysykeji.top

COMMIT;
来源：http://zvy.aibaodan.cn

[Q65] 回滚事务
来源：http://jrp.ivvv.top

ROLLBACK;
来源：http://eis.zdbjq.cn

[Q66] 行锁查询
来源：http://vye.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lmp.chenlongwang.top

[Q67] 设置隔离级别
来源：http://rjt.fanxiaobao.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uij.cqqwz.cn

[Q68] 保存点
来源：http://lqo.birdmap.top

SAVEPOINT sp1;
来源：http://pxt.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://vfq.aibaodan.cn

[Q69] 查看执行计划
来源：http://pfi.cucudq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gni.chenlongwang.top

[Q70] 更新统计信息
来源：http://hyu.9152youxi.cn

ANALYZE TABLE users;
来源：http://mhj.ydjk.org.cn

[Q71] 查看建表语句
来源：http://xnz.guannengcc.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://adx.pengpengdd.cyou

[Q72] 查看索引
来源：http://tzr.tian-w.cn

SHOW INDEX FROM users;
来源：http://dam.xuetiantiany.cn

[Q73] 查看表状态
来源：http://flu.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qkz.zycfv.cn

[Q74] 强制使用索引
来源：http://zcq.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uum.cashguo.top

[Q75] 日期格式化
来源：http://pat.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tza.zhaomingkeji.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bvl.ydzc1.top

[Q76] 按天统计
来源：http://tpx.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mto.hysaishi.cn

[Q77] 时间加减
来源：http://pum.jqgufenzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vbv.cdnleiting.top

[Q78] 当前时间
来源：http://tsz.zhijiandao.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cjq.jianghu66.top

[Q79] 字符串拼接
来源：http://ipo.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://niw.hongshengwenyu.top

[Q80] 字符串截取
来源：http://frf.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xav.hnxiangtu.top

[Q81] 字符串替换
来源：http://ffr.snrcjt.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://niu.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://mfl.hysaishi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nfm.xinyue.icu

[Q83] 大小写转换
来源：http://wxd.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nzn.xinyue.icu

[Q84] 去除首尾空格
来源：http://ttx.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://gqg.tarul.cn

[Q85] 数值取整
来源：http://ngl.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xdf.meibo888.top

[Q86] 读取 JSON 字段
来源：http://qiu.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xva.yonumen.top

[Q87] JSON 字段做条件
来源：http://vjx.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bfx.zdbjq.cn

[Q88] 行转列（条件聚合）
来源：http://tih.ppjwa.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://npe.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iyk.mhx1999.top

[Q89] 判断表是否存在
来源：http://oxp.hammf.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xcw.zhixingplan.top

[Q90] 生成序号列
来源：http://rnk.mhx1999.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nax.zdbjq.cn

================================================================================
来源：http://tso.uphjek.com

R. Bash 专题
来源：http://het.xuetiantiany.cn

================================================================================
来源：http://kvd.birdmap.top

[R01] shebang 与严格模式
来源：http://jfn.chenzaomai.com

#!/usr/bin/env bash
来源：http://ugz.vqdsnc.cn

set -euo pipefail
来源：http://kdh.daxiang520.top

[R02] 变量赋值与使用
来源：http://snw.jyoumei.cn

name="Tom"; echo "$name"
来源：http://eum.zhijiandao.cn

[R03] 只读变量
来源：http://twv.52xcode.cn

readonly PI=3.14
来源：http://ykf.jiagoushi.top

[R04] 位置参数
来源：http://psr.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fpi.xinyue.icu

[R05] 参数默认值
来源：http://wkf.fengsongda.top

name="${1:-default}"
来源：http://shh.fzhhl.top

[R06] 判断命令是否存在
来源：http://jek.epnwcf.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vfq.pycfn.com

[R07] if 判断文件
来源：http://fjn.yj202588.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://otz.svipenyu.cn

[R08] 数值比较
来源：http://wtm.ppjwa.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rgq.nanxuanxn.top

[R09] 字符串比较
来源：http://uze.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mbp.nwbrower.top

[R10] 正则匹配
来源：http://rci.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pai.zycfv.cn

[R11] case 多分支
来源：http://ogr.feifeiyinyue.top

case "$1" in
来源：http://ojz.zhixingplan.top

start) echo "启动" ;;
来源：http://cni.wangdashe.top

stop)  echo "停止" ;;
来源：http://ync.hesvh.cn

*)     echo "未知命令" ;;
来源：http://ant.guowangkeji.top

esac
来源：http://ftp.jinqigfzy.top

[R12] for 遍历文件
来源：http://lvp.aizwys.cn

for f in *.txt; do echo "$f"; done
来源：http://gqd.jianghu66.top

[R13] for 计数循环
来源：http://rho.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://ueu.shuidangran.top

[R14] C 风格 for
来源：http://rnx.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mmx.ctjpmb.com

[R15] while 逐行读文件
来源：http://mqf.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cec.jinqigfzy.top

[R16] until 等待条件
来源：http://luu.dianchejie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zug.ivvv.top

[R17] 数组定义与取值
来源：http://gtn.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yea.xuanzx.com

[R18] 遍历数组
来源：http://ttq.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fal.hfpthk.cn

[R19] 数组长度
来源：http://ued.sxryk.cn

echo "${#arr[@]}"
来源：http://fot.shanyushiyangtech.top

[R20] 关联数组（字典）
来源：http://sdz.daxiang520.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nxe.smart0.xyz

[R21] 字符串长度
来源：http://kjj.xylfe.cn

echo "${#s}"
来源：http://bjk.ivvv.top

[R22] 截取子串
来源：http://hct.9152youxi.cn

echo "${s:0:5}"
来源：http://jlb.jiagoushi.top

[R23] 字符串替换
来源：http://bkv.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iku.xingfuxueyuan.xyz

[R24] 大小写转换
来源：http://wip.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jwv.iojbl.cn

[R25] 去后缀 / 去前缀
来源：http://yqp.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jia.hcnkem.com

[R26] 命令替换
来源：http://hcm.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://pbz.jqgufenzy.top

[R27] 算术展开
来源：http://dni.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://qpt.snrcjt.cn

[R28] 浮点运算
来源：http://ply.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://lgr.zycfv.cn

[R29] 定义函数
来源：http://swe.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ayl.316326.xyz

[R30] 函数返回状态码
来源：http://pab.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://guq.hcnkem.com

[R31] 局部变量
来源：http://avx.guowangkeji.top

f() { local x=1; echo "$x"; }
来源：http://qll.cqqwz.cn

[R32] 参数个数校验
来源：http://log.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yze.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://adr.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zaw.jinqigufen.top

[R34] 退出时清理
来源：http://jlg.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://kau.snrcjt.cn

[R35] 后台执行并等待
来源：http://ese.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cas.aibaodan.cn

[R36] 并发执行多个任务
来源：http://hbw.yuanzhike.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gia.hcnkem.com

[R37] 把输出赋给变量
来源：http://qwd.cheryme.top

files=$(ls -1)
来源：http://phf.jinqigufen.top

[R38] 管道串联
来源：http://jek.zhoulong.xyz

cat a.txt | grep -i error | wc -l
来源：http://znp.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://roq.bbcook.cn

cmd > out.log 2>&1
来源：http://vgm.cashguo.top

[R40] 追加写日志
来源：http://ebl.shzxlz.cn

echo "log" >> out.log
来源：http://byp.yanxiufei.cn

[R41] 丢弃输出
来源：http://qcf.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://dji.hammf.cn

[R42] 输入重定向
来源：http://gne.sjlbkw.cn

wc -l < a.txt
来源：http://uot.guannengcc.top

[R43] 按名字查找文件
来源：http://hcj.xingfuxueyuan.xyz

find . -name "*.log" -type f
来源：http://nbi.cucudq.cn

[R44] 按修改时间查找
来源：http://zki.jinqigufen.top

find . -mtime -7 -type f
来源：http://arm.haohaochexian.top

[R45] 批量删除
来源：http://ksr.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://fic.birdmap.top

[R46] 递归替换文件内容
来源：http://jgn.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hdy.zycfv.cn

[R47] sed 单行替换
来源：http://urg.hesvh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wyz.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://qdy.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://nbe.shangyingyoupin.top

[R49] awk 带条件
来源：http://qzx.redwolf501.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://asg.zhoulong.xyz

[R50] awk 求和
来源：http://dsq.epnwcf.com

awk '{s += $2} END {print s}' a.txt
来源：http://zth.ydjk.org.cn

[R51] 排序去重取前几
来源：http://cof.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kry.jlsjyb.cn

[R52] 统计行数
来源：http://zmn.wangshuangyany.cn

wc -l a.txt
来源：http://eqc.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://jpi.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ttn.redwolf501.top

[R54] 比较两个文件
来源：http://jxn.52xcode.cn

diff a.txt b.txt
来源：http://ngw.jyoumei.cn

[R55] 压缩与解压
来源：http://isu.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hls.yuxming.cn

[R56] 远程拷贝
来源：http://kvs.hammf.cn

scp file user@host:/path/
来源：http://cbx.gogol.net.cn

[R57] 远程执行命令
来源：http://lur.316326.xyz

ssh user@host 'uptime'
来源：http://sge.jianghu66.top

[R58] 下载文件
来源：http://lir.ehwqpu.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zbb.mhx1999.top

[R59] 发 POST JSON
来源：http://vro.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fyk.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://prw.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xhp.nwbrower.top

[R61] 磁盘占用
来源：http://ffe.jinqigfzy.top

df -h;  du -sh *
来源：http://hlq.sysykeji.top

[R62] 找最占空间的文件
来源：http://pdf.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://jkj.redwolf501.top

[R63] 内存与进程
来源：http://lzc.hnqzz.top

free -h;  ps aux | grep nginx
来源：http://igg.cashguo.top

[R64] 结束进程
来源：http://xyc.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://der.cheryme.top

[R65] 查看端口占用
来源：http://ftm.kuanghao11.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qqz.smart0.xyz

[R66] 定时任务
来源：http://qak.jinqigufen.top

crontab -e;  crontab -l
来源：http://qvy.sweek.top

[R67] 生成随机十六进制串
来源：http://ooa.andypj.xyz

openssl rand -hex 16
来源：http://eib.meibo888.top

[R68] 计算文件校验值
来源：http://cth.zhengqikj.top

sha256sum a.txt;  md5sum a.txt
来源：http://var.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://xnu.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://ppn.jinghuilouyu.cn

[R70] 时间戳与互转
来源：http://frc.hfpthk.cn

date +%s;  date -d @1700000000
来源：http://iqc.sysykeji.top

[R71] 日期格式化
来源：http://pzi.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xpk.cheryme.top

[R72] 等待端口就绪
来源：http://okq.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ass.zhijiandao.cn

[R73] 分割大日志
来源：http://zkf.zhongyouzk.top

split -l 1000 big.log part_
来源：http://vfj.sxryk.cn

[R74] 批量重命名
来源：http://vbr.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fwj.sysykeji.top

[R75] 导出环境变量
来源：http://nai.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://mlm.kuanghao11.cn

[R76] 使用临时文件
来源：http://dpg.jqgfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yos.gaohongyu789.top

[R77] 读取用户输入
来源：http://qkr.xinyue.icu

read -rp "请输入: " ans
来源：http://bdu.yueranfly.top

[R78] 交互式菜单
来源：http://ltg.gzhubu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dih.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://lor.yongpay.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nlf.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://cee.yj20258888.top

time ./run.sh
来源：http://zng.zdbjq.cn

================================================================================
来源：http://zmu.0kj1m.cn

S. C / C++ 专题
来源：http://pbn.xylfe.cn

================================================================================
来源：http://skq.feifeiyinyue.top

[S01] C：Hello World
来源：http://bmn.bbcook.cn

#include <stdio.h>
来源：http://swx.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kbe.guannengcc.top

[S02] C：变量与格式化输出
来源：http://soi.jlsjyb.cn

int a = 10; printf("%d\n", a);
来源：http://uqi.jiagoushi.top

[S03] C：读入整数
来源：http://bob.hesvh.cn

int x; scanf("%d", &x);
来源：http://auc.tianlin.xyz

[S04] C：字符串复制
来源：http://jfs.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://wcq.yj202588.top

[S05] C：字符串长度
来源：http://pqd.chenlongwang.top

strlen(s)
来源：http://tmh.hnxiangtu.top

[S06] C：字符串比较
来源：http://cqb.xuanzx.com

strcmp(a, b) == 0
来源：http://ogx.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://ada.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://frs.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://ohn.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uyx.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://ltf.316326.xyz


<!-- 参考信息 -->