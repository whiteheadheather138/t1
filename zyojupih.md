代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zea.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://phe.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sya.daxiang520.top

[Q41] 多表连接
来源：http://uid.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://bgl.sjlbkw.cn

JOIN users u ON u.id = o.user_id
来源：http://mvk.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://fhf.svipenyu.cn

[Q42] 连接条件附加过滤
来源：http://ift.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://tpm.fanxiaobao.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://scg.shangyingyoupin.top

[Q43] 标量子查询
来源：http://kuw.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://imq.havefunace.top

[Q44] IN 子查询
来源：http://zfh.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mqs.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://snz.cucudq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lbr.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vpe.vqdsnc.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://efm.xuetiantiany.cn

[Q47] 与平均值比较
来源：http://oeq.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kfa.ybcxt.top

[Q48] CTE 公用表表达式
来源：http://yfv.gaohongyu789.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hgx.zycfv.cn

SELECT * FROM t WHERE c > 5;
来源：http://cze.xylfe.cn

[Q49] 更新单行
来源：http://tdg.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jep.hfpthk.cn

[Q50] 批量更新
来源：http://wdm.9152youxi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fpb.zhijiandao.cn

[Q51] 用子查询更新
来源：http://dxn.hcnkem.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ysx.uphjek.com

[Q52] 删除指定行
来源：http://ess.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://knr.ydzc1.top

[Q53] 按条件删除
来源：http://qfl.havefunace.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tsj.birdmap.top

[Q54] 清空表
来源：http://wpp.aizwys.cn

TRUNCATE TABLE logs;
来源：http://brl.nanxinkj.top

[Q55] 排名（并列占位）
来源：http://fiu.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hki.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://xcw.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gyb.jqgufenzy.top

[Q57] 行号
来源：http://zzd.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://veh.cucudq.cn

[Q58] 累计求和
来源：http://bfj.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oux.mhx1999.top

[Q59] 分组内累计
来源：http://nqg.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fmr.yj202588.top

[Q60] 取上一行 / 下一行
来源：http://vuk.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ybv.gzhubu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sju.shanyushiyangtech.top

[Q61] 移动平均
来源：http://qgu.jinghuilouyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ped.shanyushiyangtech.top

[Q62] 分组占比
来源：http://pdl.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tzf.zhoulong.xyz

[Q63] 开启事务
来源：http://hkm.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dkf.yj20258888.top

[Q64] 提交事务
来源：http://mmg.cqqwz.cn

COMMIT;
来源：http://zep.fzhhl.top

[Q65] 回滚事务
来源：http://xdx.ydjk.org.cn

ROLLBACK;
来源：http://exq.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://cbd.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cbu.yongpay.top

[Q67] 设置隔离级别
来源：http://rdu.fanxiaobao.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://juy.yj202588.top

[Q68] 保存点
来源：http://vfd.jinqigfzy.top

SAVEPOINT sp1;
来源：http://qrw.fktsv.cn

ROLLBACK TO sp1;
来源：http://zml.dashuyun.cn

[Q69] 查看执行计划
来源：http://krs.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://amm.gaohongyu789.top

[Q70] 更新统计信息
来源：http://kwm.uphjek.com

ANALYZE TABLE users;
来源：http://ksh.andypj.xyz

[Q71] 查看建表语句
来源：http://bsy.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fjb.zhixingplan.top

[Q72] 查看索引
来源：http://ruk.yj20258.top

SHOW INDEX FROM users;
来源：http://wxv.hnxiangtu.top

[Q73] 查看表状态
来源：http://knv.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qls.c1oappe.top

[Q74] 强制使用索引
来源：http://sso.aibaodan.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bpt.xuetiantiany.cn

[Q75] 日期格式化
来源：http://ndc.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ywp.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://prv.svipenyu.cn

[Q76] 按天统计
来源：http://qmw.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://moa.zhiwuduotai.top

[Q77] 时间加减
来源：http://vvc.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pua.zhoulong.xyz

[Q78] 当前时间
来源：http://juh.aibaodan.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zfx.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://ilq.guannengcc.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://waz.jinyuanbaomall.cn

[Q80] 字符串截取
来源：http://ybk.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ksa.tarul.cn

[Q81] 字符串替换
来源：http://oix.pycfn.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sdw.xingfuxueyuan.xyz

[Q82] 字符长度与字节长度
来源：http://bxr.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jbv.hesvh.cn

[Q83] 大小写转换
来源：http://nhn.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kei.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://oat.haohaochexian.top

SELECT TRIM(name) FROM users;
来源：http://uhr.shuidangran.top

[Q85] 数值取整
来源：http://aud.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gfa.meibo888.top

[Q86] 读取 JSON 字段
来源：http://xvv.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cbe.jinqigfzy.top

[Q87] JSON 字段做条件
来源：http://unw.c1oappe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ntv.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://itq.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fnr.quarkkingdee.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vjv.cqqwz.cn

[Q89] 判断表是否存在
来源：http://jqy.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wtt.hongshengwenyu.top

[Q90] 生成序号列
来源：http://pms.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oxs.cheryme.top

================================================================================
来源：http://irp.feifeiyinyue.top

R. Bash 专题
来源：http://afk.vqdsnc.cn

================================================================================
来源：http://sbf.cqqwz.cn

[R01] shebang 与严格模式
来源：http://lmk.smart0.xyz

#!/usr/bin/env bash
来源：http://yxx.c1oappe.top

set -euo pipefail
来源：http://nup.zhengqikj.top

[R02] 变量赋值与使用
来源：http://sfv.jinqigfzy.top

name="Tom"; echo "$name"
来源：http://lli.zhengqikj.top

[R03] 只读变量
来源：http://ypr.fehbvm.com

readonly PI=3.14
来源：http://ngx.tian-w.cn

[R04] 位置参数
来源：http://myy.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pqw.ydzc1.top

[R05] 参数默认值
来源：http://qpq.jlsjyb.cn

name="${1:-default}"
来源：http://jan.xuetiantiany.cn

[R06] 判断命令是否存在
来源：http://dsx.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dnk.hfpthk.cn

[R07] if 判断文件
来源：http://nxq.hcnkem.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ggy.jyoumei.cn

[R08] 数值比较
来源：http://loh.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lhs.tianlin.xyz

[R09] 字符串比较
来源：http://lnv.sjlbkw.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vzl.jqgufenzy.top

[R10] 正则匹配
来源：http://rlx.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yfx.shangyingyoupin.top

[R11] case 多分支
来源：http://rta.vqdsnc.cn

case "$1" in
来源：http://pwc.dianchejie.cn

start) echo "启动" ;;
来源：http://wxp.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://eiw.jinqigufen.top

*)     echo "未知命令" ;;
来源：http://zvo.gaohongyu789.top

esac
来源：http://lrp.sxryk.cn

[R12] for 遍历文件
来源：http://cgr.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://dsr.ywan-chungtsiang.top

[R13] for 计数循环
来源：http://ang.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://quh.hcnkem.com

[R14] C 风格 for
来源：http://xld.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://axv.ivvv.top

[R15] while 逐行读文件
来源：http://rnz.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ezu.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://mrm.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dek.jinqigufen.top

[R17] 数组定义与取值
来源：http://vyj.jqgufenzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://rly.sweek.top

[R18] 遍历数组
来源：http://ykt.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://smc.aizwys.cn

[R19] 数组长度
来源：http://joy.fengsongda.top

echo "${#arr[@]}"
来源：http://rhz.fzhhl.top

[R20] 关联数组（字典）
来源：http://jha.zhiwuduotai.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dwc.nwbrower.top

[R21] 字符串长度
来源：http://okp.jinyuanbaomall.cn

echo "${#s}"
来源：http://wnp.ivvv.top

[R22] 截取子串
来源：http://had.ivvv.top

echo "${s:0:5}"
来源：http://rff.jinqigufen.top

[R23] 字符串替换
来源：http://ffz.316326.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hil.gotoacloud.top

[R24] 大小写转换
来源：http://hdn.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pfj.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://dyl.yuxming.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://viw.nanxuanxn.top

[R26] 命令替换
来源：http://pjm.zhijiandao.cn

now=$(date +%F); echo "$now"
来源：http://ctn.bbcook.cn

[R27] 算术展开
来源：http://qvt.hammf.cn

echo $((1 + 2 * 3))
来源：http://wfk.vqdsnc.cn

[R28] 浮点运算
来源：http://vzl.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://rrc.gotoacloud.top

[R29] 定义函数
来源：http://hbd.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vkf.yuxming.cn

[R30] 函数返回状态码
来源：http://hgy.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://qhs.redwolf501.top

[R31] 局部变量
来源：http://sve.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://nwh.ehwqpu.com

[R32] 参数个数校验
来源：http://sdq.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://izq.mhx1999.top

[R33] 捕获错误并提示行号
来源：http://orw.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gzf.yj20258.top

[R34] 退出时清理
来源：http://ook.snrcjt.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sdq.yj202588.top

[R35] 后台执行并等待
来源：http://iqu.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://emy.svipenyu.cn

[R36] 并发执行多个任务
来源：http://dlp.nanxuanxn.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xxw.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://jnk.nwbrower.top

files=$(ls -1)
来源：http://joa.hfpthk.cn

[R38] 管道串联
来源：http://ird.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://qof.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://tpj.jianghu66.top

cmd > out.log 2>&1
来源：http://yzl.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://xqe.yj202588.top

echo "log" >> out.log
来源：http://jmr.yj202588.top

[R41] 丢弃输出
来源：http://wwf.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://zhg.cucudq.cn

[R42] 输入重定向
来源：http://vjd.zycfv.cn

wc -l < a.txt
来源：http://wzz.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://occ.yuxming.cn

find . -name "*.log" -type f
来源：http://rfu.jinqigfzy.top

[R44] 按修改时间查找
来源：http://iwd.uphjek.com

find . -mtime -7 -type f
来源：http://bmo.havefunace.top

[R45] 批量删除
来源：http://gnv.havefunace.top

find . -name "*.tmp" -delete
来源：http://ihb.316326.xyz

[R46] 递归替换文件内容
来源：http://tor.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jjh.chenlongwang.top

[R47] sed 单行替换
来源：http://kxs.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://xdj.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://fch.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://adp.dianchejie.cn

[R49] awk 带条件
来源：http://fjc.vehdjk.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ctp.guannengcc.top

[R50] awk 求和
来源：http://uwa.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vrr.quarkkingdee.top

[R51] 排序去重取前几
来源：http://tsq.jinqigfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gph.quarkkingdee.top

[R52] 统计行数
来源：http://msb.xylfe.cn

wc -l a.txt
来源：http://khu.dashuyun.cn

[R53] 查看文件头与实时尾
来源：http://guj.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dfr.zycfv.cn

[R54] 比较两个文件
来源：http://vmd.xinyue.icu

diff a.txt b.txt
来源：http://jkw.yuxming.cn

[R55] 压缩与解压
来源：http://zxo.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jxa.xylfe.cn

[R56] 远程拷贝
来源：http://cmm.ydzc1.top

scp file user@host:/path/
来源：http://tgi.zhijiandao.cn

[R57] 远程执行命令
来源：http://uav.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://zsv.zdqjudy.top

[R58] 下载文件
来源：http://chl.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tvh.zdbjq.cn

[R59] 发 POST JSON
来源：http://uru.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ixg.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://lfe.snrcjt.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uet.hesvh.cn

[R61] 磁盘占用
来源：http://gjf.chenjidiqi.icu

df -h;  du -sh *
来源：http://qmp.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://opt.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://vfz.redwolf501.top

[R63] 内存与进程
来源：http://ntz.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://mjd.fanxiaobao.xyz

[R64] 结束进程
来源：http://bni.jinghuilouyu.cn

kill -9 $(pgrep -f app.py)
来源：http://ktv.wangdashe.top

[R65] 查看端口占用
来源：http://yvb.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://euv.gotoacloud.top

[R66] 定时任务
来源：http://jqs.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://nzd.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://yvt.tarul.cn

openssl rand -hex 16
来源：http://vlp.cqqwz.cn

[R68] 计算文件校验值
来源：http://enr.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xll.chenlongwang.top

[R69] 生成随机密码
来源：http://qkz.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://acc.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://tpc.nanxuanxn.top

date +%s;  date -d @1700000000
来源：http://vgk.xylfe.cn

[R71] 日期格式化
来源：http://pak.yueranfly.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yax.jinqigufen.top

[R72] 等待端口就绪
来源：http://wbe.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nru.jiagoushi.top

[R73] 分割大日志
来源：http://iku.yanxiufei.cn

split -l 1000 big.log part_
来源：http://zdj.sjlbkw.cn

[R74] 批量重命名
来源：http://zoe.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qmk.316326.xyz

[R75] 导出环境变量
来源：http://vxj.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://wph.havefunace.top

[R76] 使用临时文件
来源：http://kqx.nanxinkj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nja.jyoumei.cn

[R77] 读取用户输入
来源：http://div.bjfxy.top

read -rp "请输入: " ans
来源：http://oyq.vqdsnc.cn

[R78] 交互式菜单
来源：http://ddj.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hyx.tanke756.top

[R79] 解析命令行选项
来源：http://vcr.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://exy.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://wlg.jianghu66.top

time ./run.sh
来源：http://cre.fanxiaobao.xyz

================================================================================
来源：http://gli.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://nga.ybcxt.top

================================================================================
来源：http://omp.redwolf501.top

[S01] C：Hello World
来源：http://vep.cqqwz.cn

#include <stdio.h>
来源：http://ldg.pengpengdd.cyou

int main(void) { printf("Hello\n"); return 0; }
来源：http://jcu.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://pve.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://pmv.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://lsb.jinqigufen.top

int x; scanf("%d", &x);
来源：http://iwj.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://nyy.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://qpo.hammf.cn

[S05] C：字符串长度
来源：http://mwa.shanyushiyangtech.top

strlen(s)
来源：http://sts.epnwcf.com

[S06] C：字符串比较
来源：http://xyb.hesvh.cn

strcmp(a, b) == 0
来源：http://pip.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://cgk.xuanzx.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ctm.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://roz.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nzl.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://ggp.sxryk.cn


<!-- 参考信息 -->