代发 wailian999

[Q48] CTE 公用表表达式
来源：http://iqg.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yyg.gogol.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://idi.52xcode.cn

[Q49] 更新单行
来源：http://zza.jinghuilouyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://leb.quarkkingdee.top

[Q50] 批量更新
来源：http://tox.daxiang520.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hri.hnxiangtu.top

[Q51] 用子查询更新
来源：http://lps.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dqh.zhixingplan.top

[Q52] 删除指定行
来源：http://pcj.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://sfm.havefunace.top

[Q53] 按条件删除
来源：http://hph.yongpay.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rvv.snrcjt.cn

[Q54] 清空表
来源：http://jzx.guowangkeji.top

TRUNCATE TABLE logs;
来源：http://fvy.pycfn.com

[Q55] 排名（并列占位）
来源：http://ava.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qbi.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://nbs.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bci.yfazqb.com

[Q57] 行号
来源：http://zaq.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lom.vqdsnc.cn

[Q58] 累计求和
来源：http://ffk.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wbu.hcnkem.com

[Q59] 分组内累计
来源：http://yzh.yueranfly.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nmu.ehwqpu.com

[Q60] 取上一行 / 下一行
来源：http://iah.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nfo.andypj.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sly.andypj.xyz

[Q61] 移动平均
来源：http://fee.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wbp.shanyushiyangtech.top

[Q62] 分组占比
来源：http://fuo.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jdr.vehdjk.com

[Q63] 开启事务
来源：http://tpq.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dqo.ppjwa.cn

[Q64] 提交事务
来源：http://ziw.zhengqikj.top

COMMIT;
来源：http://ami.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://qjn.fehbvm.com

ROLLBACK;
来源：http://tej.shzxlz.cn

[Q66] 行锁查询
来源：http://vlc.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ltz.guowangkeji.top

[Q67] 设置隔离级别
来源：http://uwi.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lpl.guowangkeji.top

[Q68] 保存点
来源：http://rli.shanyushiyangkeji.top

SAVEPOINT sp1;
来源：http://jub.hysaishi.cn

ROLLBACK TO sp1;
来源：http://wjq.gzhubu.top

[Q69] 查看执行计划
来源：http://hsp.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qmw.dashuyun.cn

[Q70] 更新统计信息
来源：http://lcz.tianlin.xyz

ANALYZE TABLE users;
来源：http://cgx.hywenlv.cn

[Q71] 查看建表语句
来源：http://dlj.yonumen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ecj.tarul.cn

[Q72] 查看索引
来源：http://rzq.jiagoushi.top

SHOW INDEX FROM users;
来源：http://ens.sysykeji.top

[Q73] 查看表状态
来源：http://kbb.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xmp.yangfankeji.com

[Q74] 强制使用索引
来源：http://ymq.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kmh.hysaishi.cn

[Q75] 日期格式化
来源：http://ogw.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://upg.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://viz.ydzc1.top

[Q76] 按天统计
来源：http://avt.mhx1999.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lbb.tian-w.cn

[Q77] 时间加减
来源：http://cak.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mmx.ctjpmb.com

[Q78] 当前时间
来源：http://jgm.fktsv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zds.aibaodan.cn

[Q79] 字符串拼接
来源：http://zmj.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mvq.yfazqb.com

[Q80] 字符串截取
来源：http://lmj.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lsj.jianghu66.top

[Q81] 字符串替换
来源：http://cnl.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fks.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://osr.52xcode.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mik.tianlin.xyz

[Q83] 大小写转换
来源：http://inx.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://edf.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://gcq.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://ygu.aibaodan.cn

[Q85] 数值取整
来源：http://kae.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jql.yvedp.cn

[Q86] 读取 JSON 字段
来源：http://xch.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dak.ivvv.top

[Q87] JSON 字段做条件
来源：http://isb.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://amt.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://cse.aizwys.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xmx.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dgf.jqgfzy.top

[Q89] 判断表是否存在
来源：http://hgl.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hlw.ctjpmb.com

[Q90] 生成序号列
来源：http://lwt.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://foy.chenzaomai.com

================================================================================
来源：http://ezf.xuetiantiany.cn

R. Bash 专题
来源：http://btt.ppjwa.cn

================================================================================
来源：http://bmi.zdqjudy.top

[R01] shebang 与严格模式
来源：http://jac.nanxuanxn.top

#!/usr/bin/env bash
来源：http://nsm.jlsjyb.cn

set -euo pipefail
来源：http://daj.wangdashe.top

[R02] 变量赋值与使用
来源：http://joq.yangfankeji.com

name="Tom"; echo "$name"
来源：http://kjp.ehwqpu.com

[R03] 只读变量
来源：http://ugn.shanyushiyangtech.top

readonly PI=3.14
来源：http://qab.cashguo.top

[R04] 位置参数
来源：http://jmi.hysaishi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iob.fzhhl.top

[R05] 参数默认值
来源：http://wxz.mhx1999.top

name="${1:-default}"
来源：http://bce.xziqi.cn

[R06] 判断命令是否存在
来源：http://efh.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://edl.vqdsnc.cn

[R07] if 判断文件
来源：http://gym.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mmh.pengpengdd.cyou

[R08] 数值比较
来源：http://bap.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://zwf.chenzaomai.com

[R09] 字符串比较
来源：http://sni.yuanzhike.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bfe.birdmap.top

[R10] 正则匹配
来源：http://twk.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nkt.tian-w.cn

[R11] case 多分支
来源：http://ipr.gzhubu.top

case "$1" in
来源：http://egc.hammf.cn

start) echo "启动" ;;
来源：http://xii.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://vur.quarkkingdee.top

*)     echo "未知命令" ;;
来源：http://nnd.zhiwuduotai.top

esac
来源：http://xxi.hammf.cn

[R12] for 遍历文件
来源：http://bdt.xuanzx.com

for f in *.txt; do echo "$f"; done
来源：http://tkk.havefunace.top

[R13] for 计数循环
来源：http://hhe.sjlbkw.cn

for i in {1..10}; do echo "$i"; done
来源：http://fea.jinqigfzy.top

[R14] C 风格 for
来源：http://bbs.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jop.tanke756.top

[R15] while 逐行读文件
来源：http://xvp.shanyushiyangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bzr.cheryme.top

[R16] until 等待条件
来源：http://bqh.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jgx.zhengqikj.top

[R17] 数组定义与取值
来源：http://jzd.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://ldp.hysaishi.cn

[R18] 遍历数组
来源：http://afk.hfpthk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yby.ehwqpu.com

[R19] 数组长度
来源：http://dsv.bjfxy.top

echo "${#arr[@]}"
来源：http://vvi.pycfn.com

[R20] 关联数组（字典）
来源：http://ysa.shangyingyoupin.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rgm.xuanzx.com

[R21] 字符串长度
来源：http://gnw.9152youxi.cn

echo "${#s}"
来源：http://wbq.zycfv.cn

[R22] 截取子串
来源：http://lfc.daria6918.cn

echo "${s:0:5}"
来源：http://rzt.hnqzz.top

[R23] 字符串替换
来源：http://fsp.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zfb.jinqigufen.top

[R24] 大小写转换
来源：http://dde.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://ibl.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://pqt.chenjidiqi.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://htc.yvedp.cn

[R26] 命令替换
来源：http://mmz.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://bpv.jinqigufen.top

[R27] 算术展开
来源：http://vcw.yongpay.top

echo $((1 + 2 * 3))
来源：http://fyk.tian-w.cn

[R28] 浮点运算
来源：http://byp.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://prk.xziqi.cn

[R29] 定义函数
来源：http://gqi.jinyuanbaomall.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xlv.316326.xyz

[R30] 函数返回状态码
来源：http://dme.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://fyx.aizwys.cn

[R31] 局部变量
来源：http://gqw.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://ctf.hammf.cn

[R32] 参数个数校验
来源：http://umq.cdnleiting.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xtu.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://nlu.jyoumei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ves.gaohongyu789.top

[R34] 退出时清理
来源：http://lny.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ynd.hesvh.cn

[R35] 后台执行并等待
来源：http://bsv.nanxinkj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ose.jiagoushi.top

[R36] 并发执行多个任务
来源：http://yse.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gsc.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://bcu.bbcook.cn

files=$(ls -1)
来源：http://kbv.yonumen.top

[R38] 管道串联
来源：http://hqy.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://ypj.yueranfly.top

[R39] 重定向标准输出与错误
来源：http://ljg.shangyingyoupin.top

cmd > out.log 2>&1
来源：http://xlt.9152youxi.cn

[R40] 追加写日志
来源：http://pbo.hysaishi.cn

echo "log" >> out.log
来源：http://mlj.ybcxt.top

[R41] 丢弃输出
来源：http://gbe.bbcook.cn

cmd >/dev/null 2>&1
来源：http://ywu.shangyingyoupin.top

[R42] 输入重定向
来源：http://stx.sjlbkw.cn

wc -l < a.txt
来源：http://byx.fktsv.cn

[R43] 按名字查找文件
来源：http://vch.kuanghao11.cn

find . -name "*.log" -type f
来源：http://vkj.yuanzhike.top

[R44] 按修改时间查找
来源：http://qvm.ppjwa.cn

find . -mtime -7 -type f
来源：http://piw.zdqjudy.top

[R45] 批量删除
来源：http://zvu.xuanzx.com

find . -name "*.tmp" -delete
来源：http://lxm.gzhubu.top

[R46] 递归替换文件内容
来源：http://ckj.9152youxi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xsc.chenlongwang.top

[R47] sed 单行替换
来源：http://yje.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://gas.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://bjr.ppjwa.cn

awk '{print $1, $3}' a.txt
来源：http://wus.sufxvd.cn

[R49] awk 带条件
来源：http://fjm.jianghu66.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ahy.hywenlv.cn

[R50] awk 求和
来源：http://myr.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://odv.cdnleiting.top

[R51] 排序去重取前几
来源：http://upx.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qfm.meibo888.top

[R52] 统计行数
来源：http://bhg.hywenlv.cn

wc -l a.txt
来源：http://ojw.havefunace.top

[R53] 查看文件头与实时尾
来源：http://tbg.sxryk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qak.ivvv.top

[R54] 比较两个文件
来源：http://bcf.xinyue.icu

diff a.txt b.txt
来源：http://emk.ctjpmb.com

[R55] 压缩与解压
来源：http://iwb.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pit.jqgufenzy.top

[R56] 远程拷贝
来源：http://skg.yuxming.cn

scp file user@host:/path/
来源：http://xsw.andypj.xyz

[R57] 远程执行命令
来源：http://bxc.yangfankeji.com

ssh user@host 'uptime'
来源：http://nwd.wangdashe.top

[R58] 下载文件
来源：http://vho.hywenlv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ywc.ydjk.org.cn

[R59] 发 POST JSON
来源：http://sjl.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xiq.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://wny.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dok.tanke756.top

[R61] 磁盘占用
来源：http://vry.9152youxi.cn

df -h;  du -sh *
来源：http://hwr.cqqwz.cn

[R62] 找最占空间的文件
来源：http://aly.fehbvm.com

du -ah . | sort -rh | head -10
来源：http://isc.zhoulong.xyz

[R63] 内存与进程
来源：http://liz.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://iwr.hnxiangtu.top

[R64] 结束进程
来源：http://dle.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://cna.yfazqb.com

[R65] 查看端口占用
来源：http://yrh.cqqwz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://urr.meibo888.top

[R66] 定时任务
来源：http://ksp.gotoacloud.top

crontab -e;  crontab -l
来源：http://fuu.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://idr.jianghu66.top

openssl rand -hex 16
来源：http://nxp.yvedp.cn

[R68] 计算文件校验值
来源：http://jqb.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://dwe.dianchejie.cn

[R69] 生成随机密码
来源：http://wmw.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://zfb.fehbvm.com

[R70] 时间戳与互转
来源：http://mxu.pycfn.com

date +%s;  date -d @1700000000
来源：http://hyr.epnwcf.com

[R71] 日期格式化
来源：http://gke.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://htm.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://yea.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fnx.fzhhl.top

[R73] 分割大日志
来源：http://zqd.yfazqb.com

split -l 1000 big.log part_
来源：http://usj.chenjidiqi.icu

[R74] 批量重命名
来源：http://hhr.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jlu.shzxlz.cn

[R75] 导出环境变量
来源：http://uso.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://zbn.birdmap.top

[R76] 使用临时文件
来源：http://ibr.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ciz.yj202588.top

[R77] 读取用户输入
来源：http://rxr.zycfv.cn

read -rp "请输入: " ans
来源：http://uav.sufxvd.cn

[R78] 交互式菜单
来源：http://frr.shanyushiyangtech.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kzr.jinqigfzy.top

[R79] 解析命令行选项
来源：http://cui.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qqz.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://wdq.daria6918.cn

time ./run.sh
来源：http://lvi.snrcjt.cn

================================================================================
来源：http://dna.ywan-chungtsiang.top

S. C / C++ 专题
来源：http://sse.nanxinkj.top

================================================================================
来源：http://lce.xziqi.cn

[S01] C：Hello World
来源：http://dwx.zdbjq.cn

#include <stdio.h>
来源：http://jhq.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://now.fanxiaobao.xyz

[S02] C：变量与格式化输出
来源：http://odx.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://uyf.fktsv.cn

[S03] C：读入整数
来源：http://twp.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://wea.iojbl.cn

[S04] C：字符串复制
来源：http://gck.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://gfj.shangyingyoupin.top

[S05] C：字符串长度
来源：http://pzq.snrcjt.cn

strlen(s)
来源：http://nub.0kj1m.cn

[S06] C：字符串比较
来源：http://kcz.jlsjyb.cn

strcmp(a, b) == 0
来源：http://ywh.hywenlv.cn

[S07] C：数组遍历求和
来源：http://wpn.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iyj.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://dtd.yueranfly.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dky.aibaodan.cn

[S09] C：结构体定义与初始化
来源：http://and.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vso.snrcjt.cn

[S10] C：指针与解引用
来源：http://zxy.hesvh.cn

int *p = &a;  *p = 5;
来源：http://xec.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://ldf.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://rrr.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mpy.aibaodan.cn

fclose(f);
来源：http://yuw.fktsv.cn

[S12] C：写文件
来源：http://nbv.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bxr.ehwqpu.com

[S13] C：宏定义
来源：http://gaw.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gsh.jinqigufen.top

[S14] C：枚举
来源：http://flr.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://ijn.sweek.top

[S15] C：类型转换
来源：http://fnd.fehbvm.com

(double) a / b
来源：http://jzl.zhengqikj.top

[S16] C：位操作置位
来源：http://got.cucudq.cn

x |= (1 << 3);
来源：http://atf.yongpay.top

[S17] C：安全拼接字符串
来源：http://std.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pqs.jyoumei.cn

[S18] C：命令行参数
来源：http://goz.hywenlv.cn


<!-- 参考信息 -->