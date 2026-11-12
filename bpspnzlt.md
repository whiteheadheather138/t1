代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://gpw.sweek.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rfo.chenlongwang.top

[Q47] 与平均值比较
来源：http://hib.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lyi.sweek.top

[Q48] CTE 公用表表达式
来源：http://cwq.aizwys.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hnd.epnwcf.com

SELECT * FROM t WHERE c > 5;
来源：http://enp.yfazqb.com

[Q49] 更新单行
来源：http://qqz.fanxiaobao.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://trk.svipenyu.cn

[Q50] 批量更新
来源：http://txz.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aon.hfpthk.cn

[Q51] 用子查询更新
来源：http://mtk.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wus.yuxming.cn

[Q52] 删除指定行
来源：http://vhh.yfazqb.com

DELETE FROM users WHERE id = 10;
来源：http://ack.tianlin.xyz

[Q53] 按条件删除
来源：http://yfl.yvedp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ngt.shangyingyoupin.top

[Q54] 清空表
来源：http://kfg.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://tyc.tian-w.cn

[Q55] 排名（并列占位）
来源：http://npn.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ruo.316326.xyz

[Q56] 密集排名（并列不占位）
来源：http://xll.daria6918.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gnn.jqgfzy.top

[Q57] 行号
来源：http://esw.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uuv.vqdsnc.cn

[Q58] 累计求和
来源：http://esv.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kjx.yuanzhike.top

[Q59] 分组内累计
来源：http://xek.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sdw.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://ioc.xuetiantiany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ijz.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gpq.c1oappe.top

[Q61] 移动平均
来源：http://fyq.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mlv.hnxiangtu.top

[Q62] 分组占比
来源：http://lsn.quarkkingdee.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ncf.hammf.cn

[Q63] 开启事务
来源：http://olg.xuanzx.com

START TRANSACTION;                -- 或 BEGIN
来源：http://bvl.yuxming.cn

[Q64] 提交事务
来源：http://hfh.hysaishi.cn

COMMIT;
来源：http://wit.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://tkr.cucudq.cn

ROLLBACK;
来源：http://yxh.tianlin.xyz

[Q66] 行锁查询
来源：http://pnd.hammf.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ykz.c1oappe.top

[Q67] 设置隔离级别
来源：http://zpc.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gxu.yueranfly.top

[Q68] 保存点
来源：http://gxw.sxryk.cn

SAVEPOINT sp1;
来源：http://esa.yvedp.cn

ROLLBACK TO sp1;
来源：http://yvf.ybcxt.top

[Q69] 查看执行计划
来源：http://bhi.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://czy.ivvv.top

[Q70] 更新统计信息
来源：http://utm.chenjidiqi.icu

ANALYZE TABLE users;
来源：http://lun.shzxlz.cn

[Q71] 查看建表语句
来源：http://wln.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zhj.ivvv.top

[Q72] 查看索引
来源：http://lkc.yvedp.cn

SHOW INDEX FROM users;
来源：http://hrj.jinqigfzy.top

[Q73] 查看表状态
来源：http://rbs.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://mkv.jlsjyb.cn

[Q74] 强制使用索引
来源：http://xhx.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://alh.zhixingplan.top

[Q75] 日期格式化
来源：http://ybo.chenlongwang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hrh.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aik.guowangkeji.top

[Q76] 按天统计
来源：http://ukc.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ndx.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://duo.yongpay.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ote.c1oappe.top

[Q78] 当前时间
来源：http://wxh.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://koa.jianghu66.top

[Q79] 字符串拼接
来源：http://pgq.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bpb.ybcxt.top

[Q80] 字符串截取
来源：http://jis.pengpengdd.cyou

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dpz.hnxiangtu.top

[Q81] 字符串替换
来源：http://egf.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hly.birdmap.top

[Q82] 字符长度与字节长度
来源：http://odi.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rpd.chenzaomai.com

[Q83] 大小写转换
来源：http://jhf.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kog.nwbrower.top

[Q84] 去除首尾空格
来源：http://cdt.jinqigfzy.top

SELECT TRIM(name) FROM users;
来源：http://amn.gaohongyu789.top

[Q85] 数值取整
来源：http://jrq.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eut.smart0.xyz

[Q86] 读取 JSON 字段
来源：http://bpg.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rbi.jinghuilouyu.cn

[Q87] JSON 字段做条件
来源：http://sjt.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cvl.hfpthk.cn

[Q88] 行转列（条件聚合）
来源：http://hhy.ctjpmb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zsv.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aap.cashguo.top

[Q89] 判断表是否存在
来源：http://ick.chenjidiqi.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hzy.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://mkk.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zde.fzhhl.top

================================================================================
来源：http://wht.52xcode.cn

R. Bash 专题
来源：http://vxy.chenjidiqi.icu

================================================================================
来源：http://wym.daxiang520.top

[R01] shebang 与严格模式
来源：http://xzl.cheryme.top

#!/usr/bin/env bash
来源：http://eqa.uphjek.com

set -euo pipefail
来源：http://osq.fktsv.cn

[R02] 变量赋值与使用
来源：http://iia.yangfankeji.com

name="Tom"; echo "$name"
来源：http://iyu.tanke756.top

[R03] 只读变量
来源：http://rox.pengpengdd.cyou

readonly PI=3.14
来源：http://rlf.aizwys.cn

[R04] 位置参数
来源：http://ehq.havefunace.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lau.0kj1m.cn

[R05] 参数默认值
来源：http://zlf.cdnleiting.top

name="${1:-default}"
来源：http://tof.sufxvd.cn

[R06] 判断命令是否存在
来源：http://jki.zhengqikj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dqm.hcnkem.com

[R07] if 判断文件
来源：http://ago.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://igm.cdnleiting.top

[R08] 数值比较
来源：http://toe.chenlongwang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qoc.hesvh.cn

[R09] 字符串比较
来源：http://ijl.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ltr.jinqigufen.top

[R10] 正则匹配
来源：http://vyl.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rnb.shangyingyoupin.top

[R11] case 多分支
来源：http://wmo.yuanzhike.top

case "$1" in
来源：http://eku.cdnleiting.top

start) echo "启动" ;;
来源：http://zaq.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://wip.daxiang520.top

*)     echo "未知命令" ;;
来源：http://jdc.xuanzx.com

esac
来源：http://gfz.uphjek.com

[R12] for 遍历文件
来源：http://tvc.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://myp.jlsjyb.cn

[R13] for 计数循环
来源：http://gxz.hywenlv.cn

for i in {1..10}; do echo "$i"; done
来源：http://orn.xziqi.cn

[R14] C 风格 for
来源：http://qkl.0kj1m.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ykv.ehwqpu.com

[R15] while 逐行读文件
来源：http://lbu.fzhhl.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ejw.tianlin.xyz

[R16] until 等待条件
来源：http://eza.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iwo.yj20258888.top

[R17] 数组定义与取值
来源：http://yjy.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zmy.sufxvd.cn

[R18] 遍历数组
来源：http://rph.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ieb.yj20258888.top

[R19] 数组长度
来源：http://efr.shanyushiyangkeji.top

echo "${#arr[@]}"
来源：http://nti.svipenyu.cn

[R20] 关联数组（字典）
来源：http://vtj.52xcode.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cbd.dianchejie.cn

[R21] 字符串长度
来源：http://atz.svipenyu.cn

echo "${#s}"
来源：http://gdn.ivvv.top

[R22] 截取子串
来源：http://vzj.hfpthk.cn

echo "${s:0:5}"
来源：http://wbe.meibo888.top

[R23] 字符串替换
来源：http://tsw.uphjek.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zwl.uphjek.com

[R24] 大小写转换
来源：http://skh.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wbi.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://vtt.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lvn.nwbrower.top

[R26] 命令替换
来源：http://fxn.cheryme.top

now=$(date +%F); echo "$now"
来源：http://bdj.hcnkem.com

[R27] 算术展开
来源：http://guh.jinqigufen.top

echo $((1 + 2 * 3))
来源：http://vye.shuidangran.top

[R28] 浮点运算
来源：http://tcu.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://nxs.sjlbkw.cn

[R29] 定义函数
来源：http://usd.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dgd.zhengqikj.top

[R30] 函数返回状态码
来源：http://izf.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://ruc.hnxiangtu.top

[R31] 局部变量
来源：http://omm.shzxlz.cn

f() { local x=1; echo "$x"; }
来源：http://qiz.redwolf501.top

[R32] 参数个数校验
来源：http://bej.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qts.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://zpi.hfpthk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://doo.tarul.cn

[R34] 退出时清理
来源：http://jlu.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://gga.wangdashe.top

[R35] 后台执行并等待
来源：http://ebs.hcnkem.com

sleep 5 & pid=$!; wait "$pid"
来源：http://fls.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://fuv.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iai.xylfe.cn

[R37] 把输出赋给变量
来源：http://owt.jyoumei.cn

files=$(ls -1)
来源：http://msk.shuidangran.top

[R38] 管道串联
来源：http://rkz.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://txl.yonumen.top

[R39] 重定向标准输出与错误
来源：http://oqb.shuidangran.top

cmd > out.log 2>&1
来源：http://lfd.sjlbkw.cn

[R40] 追加写日志
来源：http://hwx.jinghuilouyu.cn

echo "log" >> out.log
来源：http://mlz.nanxinkj.top

[R41] 丢弃输出
来源：http://jod.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://uab.fktsv.cn

[R42] 输入重定向
来源：http://twq.yvedp.cn

wc -l < a.txt
来源：http://baz.pycfn.com

[R43] 按名字查找文件
来源：http://teb.cqqwz.cn

find . -name "*.log" -type f
来源：http://bpe.yongpay.top

[R44] 按修改时间查找
来源：http://ytm.yj20258.top

find . -mtime -7 -type f
来源：http://inj.jqgufenzy.top

[R45] 批量删除
来源：http://wmh.yueranfly.top

find . -name "*.tmp" -delete
来源：http://mgt.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://kfg.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mrz.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://jht.smart0.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://oqv.jinqigufen.top

[R48] awk 取指定列
来源：http://ijh.yfazqb.com

awk '{print $1, $3}' a.txt
来源：http://cdo.tanke756.top

[R49] awk 带条件
来源：http://eqo.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://psy.yuanzhike.top

[R50] awk 求和
来源：http://dyd.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://mud.aibaodan.cn

[R51] 排序去重取前几
来源：http://gxi.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://enf.zhijiandao.cn

[R52] 统计行数
来源：http://axn.zdbjq.cn

wc -l a.txt
来源：http://avd.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://mhg.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hom.shzxlz.cn

[R54] 比较两个文件
来源：http://ypf.vehdjk.com

diff a.txt b.txt
来源：http://axc.sjlbkw.cn

[R55] 压缩与解压
来源：http://eno.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://axr.feifeiyinyue.top

[R56] 远程拷贝
来源：http://uhy.yj20258.top

scp file user@host:/path/
来源：http://osr.gogol.net.cn

[R57] 远程执行命令
来源：http://cny.yonumen.top

ssh user@host 'uptime'
来源：http://meu.hnqzz.top

[R58] 下载文件
来源：http://aka.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tua.kuanghao11.cn

[R59] 发 POST JSON
来源：http://ezs.quarkkingdee.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yyw.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://wqr.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xok.vehdjk.com

[R61] 磁盘占用
来源：http://zfz.bjfxy.top

df -h;  du -sh *
来源：http://dks.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://mgs.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://igq.tarul.cn

[R63] 内存与进程
来源：http://dso.hcnkem.com

free -h;  ps aux | grep nginx
来源：http://jui.svipenyu.cn

[R64] 结束进程
来源：http://wuh.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://oyk.yj20258888.top

[R65] 查看端口占用
来源：http://yok.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mfs.cheryme.top

[R66] 定时任务
来源：http://wsp.vqdsnc.cn

crontab -e;  crontab -l
来源：http://jzd.kuanghao11.cn

[R67] 生成随机十六进制串
来源：http://xas.daxiang520.top

openssl rand -hex 16
来源：http://jcl.cashguo.top

[R68] 计算文件校验值
来源：http://bsq.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://zuw.xylfe.cn

[R69] 生成随机密码
来源：http://dhl.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://abw.jqgufenzy.top

[R70] 时间戳与互转
来源：http://vzo.daxiang520.top

date +%s;  date -d @1700000000
来源：http://czb.zhiwuduotai.top

[R71] 日期格式化
来源：http://fvp.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://brl.quarkkingdee.top

[R72] 等待端口就绪
来源：http://tuq.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nic.9152youxi.cn

[R73] 分割大日志
来源：http://isk.9152youxi.cn

split -l 1000 big.log part_
来源：http://pwy.zdbjq.cn

[R74] 批量重命名
来源：http://lih.jinqigufen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jex.dashuyun.cn

[R75] 导出环境变量
来源：http://fqb.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://vjs.hywenlv.cn

[R76] 使用临时文件
来源：http://vrr.sweek.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qmq.daxiang520.top

[R77] 读取用户输入
来源：http://sdq.hywenlv.cn

read -rp "请输入: " ans
来源：http://upd.daria6918.cn

[R78] 交互式菜单
来源：http://ikj.nwbrower.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hio.tian-w.cn

[R79] 解析命令行选项
来源：http://fyj.nanxuanxn.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gnt.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://qla.chenjidiqi.icu

time ./run.sh
来源：http://fzj.yj20258888.top

================================================================================
来源：http://ies.jiagoushi.top

S. C / C++ 专题
来源：http://kcp.fehbvm.com

================================================================================
来源：http://hyr.bjfxy.top

[S01] C：Hello World
来源：http://sxm.dashuyun.cn

#include <stdio.h>
来源：http://nvn.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://bph.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://oid.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://cat.feifeiyinyue.top

[S03] C：读入整数
来源：http://vuv.gzhubu.top

int x; scanf("%d", &x);
来源：http://jnf.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://dui.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://diw.wangdashe.top

[S05] C：字符串长度
来源：http://ngk.fanxiaobao.xyz

strlen(s)
来源：http://dcx.redwolf501.top

[S06] C：字符串比较
来源：http://ttt.nanxinkj.top

strcmp(a, b) == 0
来源：http://ebd.0kj1m.cn

[S07] C：数组遍历求和
来源：http://xhr.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tdi.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://lcm.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vmt.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://ogz.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rbi.nanxuanxn.top

[S10] C：指针与解引用
来源：http://leh.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://tmv.zhongyouzk.top

[S11] C：逐行读文件
来源：http://dou.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://ymb.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://wyi.xinyue.icu

fclose(f);
来源：http://nms.sjlbkw.cn

[S12] C：写文件
来源：http://csl.sxryk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://naf.iojbl.cn

[S13] C：宏定义
来源：http://ylt.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kzx.jlsjyb.cn

[S14] C：枚举
来源：http://uks.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://tlu.fehbvm.com

[S15] C：类型转换
来源：http://ysk.cdnleiting.top

(double) a / b
来源：http://dql.hesvh.cn

[S16] C：位操作置位
来源：http://ssm.yuanzhike.top


<!-- 参考信息 -->