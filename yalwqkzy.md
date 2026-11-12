代发 wailian999

[Q48] CTE 公用表表达式
来源：http://scm.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fcf.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://zsu.zhoulong.xyz

[Q49] 更新单行
来源：http://wfg.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fmj.gaohongyu789.top

[Q50] 批量更新
来源：http://but.yj20258888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qdh.gotoacloud.top

[Q51] 用子查询更新
来源：http://stu.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wiq.havefunace.top

[Q52] 删除指定行
来源：http://bjs.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://lss.jinqigfzy.top

[Q53] 按条件删除
来源：http://hwk.fktsv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sod.bjfxy.top

[Q54] 清空表
来源：http://kmk.chenzaomai.com

TRUNCATE TABLE logs;
来源：http://rkw.cashguo.top

[Q55] 排名（并列占位）
来源：http://hij.pycfn.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lhl.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://azr.zdbjq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qnl.gzhubu.top

[Q57] 行号
来源：http://rlz.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lzt.yj20258.top

[Q58] 累计求和
来源：http://teo.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://azy.gogol.net.cn

[Q59] 分组内累计
来源：http://pdh.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rug.sysykeji.top

[Q60] 取上一行 / 下一行
来源：http://tdg.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fpk.yongpay.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://skh.shangyingyoupin.top

[Q61] 移动平均
来源：http://glv.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rps.jiagoushi.top

[Q62] 分组占比
来源：http://vns.shanyushiyangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tpa.sjlbkw.cn

[Q63] 开启事务
来源：http://bbi.jinghuilouyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fph.andypj.xyz

[Q64] 提交事务
来源：http://hpt.ydzc1.top

COMMIT;
来源：http://poq.jlsjyb.cn

[Q65] 回滚事务
来源：http://buk.aizwys.cn

ROLLBACK;
来源：http://kgu.hysaishi.cn

[Q66] 行锁查询
来源：http://zzu.gotoacloud.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bcx.fehbvm.com

[Q67] 设置隔离级别
来源：http://wvt.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mop.kuanghao11.cn

[Q68] 保存点
来源：http://tto.xziqi.cn

SAVEPOINT sp1;
来源：http://gew.hammf.cn

ROLLBACK TO sp1;
来源：http://zmw.gogol.net.cn

[Q69] 查看执行计划
来源：http://hou.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cpi.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://bwv.dashuyun.cn

ANALYZE TABLE users;
来源：http://ppy.hywenlv.cn

[Q71] 查看建表语句
来源：http://xhp.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://max.52xcode.cn

[Q72] 查看索引
来源：http://rzi.jinghuilouyu.cn

SHOW INDEX FROM users;
来源：http://uhn.wangdashe.top

[Q73] 查看表状态
来源：http://ufi.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ayb.nanxinkj.top

[Q74] 强制使用索引
来源：http://org.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xam.tianlin.xyz

[Q75] 日期格式化
来源：http://vzu.nanxinkj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yis.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xdh.jinghuilouyu.cn

[Q76] 按天统计
来源：http://iyt.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qcy.tian-w.cn

[Q77] 时间加减
来源：http://mja.xziqi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zoj.gaohongyu789.top

[Q78] 当前时间
来源：http://qdd.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uab.zhixingplan.top

[Q79] 字符串拼接
来源：http://jrk.chenzaomai.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qmm.tanke756.top

[Q80] 字符串截取
来源：http://vrk.fanxiaobao.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mgn.pycfn.com

[Q81] 字符串替换
来源：http://fns.jqgufenzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zhu.dianchejie.cn

[Q82] 字符长度与字节长度
来源：http://iqo.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://plt.ppjwa.cn

[Q83] 大小写转换
来源：http://xuq.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pzz.c1oappe.top

[Q84] 去除首尾空格
来源：http://fge.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://vgr.svipenyu.cn

[Q85] 数值取整
来源：http://liv.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qqz.guowangkeji.top

[Q86] 读取 JSON 字段
来源：http://jmw.jinghuilouyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://djm.pycfn.com

[Q87] JSON 字段做条件
来源：http://xgh.yuxming.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wun.jiagoushi.top

[Q88] 行转列（条件聚合）
来源：http://ttt.fengsongda.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aki.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cbx.dashuyun.cn

[Q89] 判断表是否存在
来源：http://qfu.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iwx.yj20258888.top

[Q90] 生成序号列
来源：http://rxh.guowangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cwc.nanxinkj.top

================================================================================
来源：http://ruo.shzxlz.cn

R. Bash 专题
来源：http://mol.shanyushiyangtech.top

================================================================================
来源：http://trp.hnqzz.top

[R01] shebang 与严格模式
来源：http://kgx.cashguo.top

#!/usr/bin/env bash
来源：http://phb.sjlbkw.cn

set -euo pipefail
来源：http://cax.0kj1m.cn

[R02] 变量赋值与使用
来源：http://yng.nanxinkj.top

name="Tom"; echo "$name"
来源：http://lsm.zhixingplan.top

[R03] 只读变量
来源：http://cub.shangyingyoupin.top

readonly PI=3.14
来源：http://tzg.zhoulong.xyz

[R04] 位置参数
来源：http://jro.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uvm.epnwcf.com

[R05] 参数默认值
来源：http://ozw.guannengcc.top

name="${1:-default}"
来源：http://yhk.guannengcc.top

[R06] 判断命令是否存在
来源：http://sif.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xmb.hysaishi.cn

[R07] if 判断文件
来源：http://xar.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gsp.sxryk.cn

[R08] 数值比较
来源：http://dng.xingfuxueyuan.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://sac.sysykeji.top

[R09] 字符串比较
来源：http://bij.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://htv.gogol.net.cn

[R10] 正则匹配
来源：http://wlo.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xqn.hcnkem.com

[R11] case 多分支
来源：http://rsr.fzhhl.top

case "$1" in
来源：http://siv.hfpthk.cn

start) echo "启动" ;;
来源：http://tpc.hnqzz.top

stop)  echo "停止" ;;
来源：http://zxb.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://mrr.wangshuangyany.cn

esac
来源：http://jsq.cheryme.top

[R12] for 遍历文件
来源：http://uig.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://tdb.zycfv.cn

[R13] for 计数循环
来源：http://dmh.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://daz.zhengqikj.top

[R14] C 风格 for
来源：http://tyk.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://syy.vehdjk.com

[R15] while 逐行读文件
来源：http://pgt.quarkkingdee.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://per.ehwqpu.com

[R16] until 等待条件
来源：http://tto.hnqzz.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wjc.daxiang520.top

[R17] 数组定义与取值
来源：http://meo.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://ynk.yuxming.cn

[R18] 遍历数组
来源：http://bmo.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wel.sjlbkw.cn

[R19] 数组长度
来源：http://tgr.jqgfzy.top

echo "${#arr[@]}"
来源：http://uep.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://vgs.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vvj.cqqwz.cn

[R21] 字符串长度
来源：http://lac.jiagoushi.top

echo "${#s}"
来源：http://btj.kuanghao11.cn

[R22] 截取子串
来源：http://swh.yueranfly.top

echo "${s:0:5}"
来源：http://zqo.cheryme.top

[R23] 字符串替换
来源：http://bnj.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://atu.fzhhl.top

[R24] 大小写转换
来源：http://hmb.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uzp.uphjek.com

[R25] 去后缀 / 去前缀
来源：http://chu.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mtf.shuidangran.top

[R26] 命令替换
来源：http://wav.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://sma.yj20258.top

[R27] 算术展开
来源：http://zcr.jiagoushi.top

echo $((1 + 2 * 3))
来源：http://dpn.yanxiufei.cn

[R28] 浮点运算
来源：http://ifc.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://kbw.gzhubu.top

[R29] 定义函数
来源：http://ofv.shuidangran.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tmf.vqdsnc.cn

[R30] 函数返回状态码
来源：http://iyj.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://hxf.yongpay.top

[R31] 局部变量
来源：http://xys.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://dfw.dashuyun.cn

[R32] 参数个数校验
来源：http://tsx.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dou.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://zui.ydjk.org.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bbu.pycfn.com

[R34] 退出时清理
来源：http://sut.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://nap.ydjk.org.cn

[R35] 后台执行并等待
来源：http://olv.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ijr.chenlongwang.top

[R36] 并发执行多个任务
来源：http://ajw.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qfx.jinqigufen.top

[R37] 把输出赋给变量
来源：http://bwl.fanxiaobao.xyz

files=$(ls -1)
来源：http://fzg.nwbrower.top

[R38] 管道串联
来源：http://fcx.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://mnu.9152youxi.cn

[R39] 重定向标准输出与错误
来源：http://tgv.hywenlv.cn

cmd > out.log 2>&1
来源：http://gdz.hysaishi.cn

[R40] 追加写日志
来源：http://uni.nwbrower.top

echo "log" >> out.log
来源：http://fjl.aizwys.cn

[R41] 丢弃输出
来源：http://iqs.yj20258888.top

cmd >/dev/null 2>&1
来源：http://zrl.snrcjt.cn

[R42] 输入重定向
来源：http://tun.fktsv.cn

wc -l < a.txt
来源：http://nrh.chenzaomai.com

[R43] 按名字查找文件
来源：http://fre.dianchejie.cn

find . -name "*.log" -type f
来源：http://bon.chenzaomai.com

[R44] 按修改时间查找
来源：http://hlc.zhixingplan.top

find . -mtime -7 -type f
来源：http://arq.sxryk.cn

[R45] 批量删除
来源：http://ymx.tianlin.xyz

find . -name "*.tmp" -delete
来源：http://mmz.c1oappe.top

[R46] 递归替换文件内容
来源：http://sqh.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vme.zhengqikj.top

[R47] sed 单行替换
来源：http://ltx.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sro.dashuyun.cn

[R48] awk 取指定列
来源：http://lie.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://mpu.hysaishi.cn

[R49] awk 带条件
来源：http://vcz.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mst.ybcxt.top

[R50] awk 求和
来源：http://kwm.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://whc.fzhhl.top

[R51] 排序去重取前几
来源：http://ykz.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jxh.feifeiyinyue.top

[R52] 统计行数
来源：http://nbq.jqgfzy.top

wc -l a.txt
来源：http://slt.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://cjw.smart0.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zpq.daria6918.cn

[R54] 比较两个文件
来源：http://xrv.ydjk.org.cn

diff a.txt b.txt
来源：http://ggl.sjlbkw.cn

[R55] 压缩与解压
来源：http://xky.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jlf.cucudq.cn

[R56] 远程拷贝
来源：http://msk.jianghu66.top

scp file user@host:/path/
来源：http://wck.gogol.net.cn

[R57] 远程执行命令
来源：http://dhx.cqqwz.cn

ssh user@host 'uptime'
来源：http://yht.hywenlv.cn

[R58] 下载文件
来源：http://ltt.hywenlv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jka.yj202588.top

[R59] 发 POST JSON
来源：http://leq.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mzu.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://tks.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lyt.feifeiyinyue.top

[R61] 磁盘占用
来源：http://kfa.yj20258.top

df -h;  du -sh *
来源：http://cea.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://efk.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://him.shzxlz.cn

[R63] 内存与进程
来源：http://eag.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://jqu.nanxinkj.top

[R64] 结束进程
来源：http://axd.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://bpl.yangfankeji.com

[R65] 查看端口占用
来源：http://snc.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ccu.kuanghao11.cn

[R66] 定时任务
来源：http://qdg.0kj1m.cn

crontab -e;  crontab -l
来源：http://kgp.vehdjk.com

[R67] 生成随机十六进制串
来源：http://ahr.vehdjk.com

openssl rand -hex 16
来源：http://kmc.zhiwuduotai.top

[R68] 计算文件校验值
来源：http://jam.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://ozk.tarul.cn

[R69] 生成随机密码
来源：http://zwp.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://fdf.vqdsnc.cn

[R70] 时间戳与互转
来源：http://swq.hnqzz.top

date +%s;  date -d @1700000000
来源：http://glt.vqdsnc.cn

[R71] 日期格式化
来源：http://rns.yj202588.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rus.jqgufenzy.top

[R72] 等待端口就绪
来源：http://yns.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rhw.meibo888.top

[R73] 分割大日志
来源：http://cyl.snrcjt.cn

split -l 1000 big.log part_
来源：http://qxr.hysaishi.cn

[R74] 批量重命名
来源：http://drj.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://agi.xziqi.cn

[R75] 导出环境变量
来源：http://gav.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://sgf.zhaomingkeji.xyz

[R76] 使用临时文件
来源：http://wvj.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mjq.gotoacloud.top

[R77] 读取用户输入
来源：http://nnv.hcnkem.com

read -rp "请输入: " ans
来源：http://dts.sxryk.cn

[R78] 交互式菜单
来源：http://jwz.zhoulong.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://cke.xuanzx.com

[R79] 解析命令行选项
来源：http://vof.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tpi.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://dtk.cheryme.top

time ./run.sh
来源：http://ulb.ivvv.top

================================================================================
来源：http://qtq.pycfn.com

S. C / C++ 专题
来源：http://nzh.yuanzhike.top

================================================================================
来源：http://xpx.shuidangran.top

[S01] C：Hello World
来源：http://nex.shanyushiyangkeji.top

#include <stdio.h>
来源：http://hzg.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://arl.yj20258.top

[S02] C：变量与格式化输出
来源：http://ons.wangshuangyany.cn

int a = 10; printf("%d\n", a);
来源：http://tff.bjfxy.top

[S03] C：读入整数
来源：http://cfk.redwolf501.top

int x; scanf("%d", &x);
来源：http://epx.hnqzz.top

[S04] C：字符串复制
来源：http://qnh.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://sng.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://tkp.svipenyu.cn

strlen(s)
来源：http://aln.c1oappe.top

[S06] C：字符串比较
来源：http://ovz.daxiang520.top

strcmp(a, b) == 0
来源：http://ffj.zycfv.cn

[S07] C：数组遍历求和
来源：http://aab.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ehd.hnqzz.top

[S08] C：动态内存分配与释放
来源：http://neq.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hvz.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://bcj.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sxh.jqgfzy.top

[S10] C：指针与解引用
来源：http://dos.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://bjj.ydjk.org.cn

[S11] C：逐行读文件
来源：http://jcy.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://xdk.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://edh.hysaishi.cn

fclose(f);
来源：http://xvu.zhijiandao.cn

[S12] C：写文件
来源：http://bqy.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ktp.shangyingyoupin.top

[S13] C：宏定义
来源：http://vmy.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gfw.hongshengwenyu.top

[S14] C：枚举
来源：http://szq.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://zpr.chenlongwang.top

[S15] C：类型转换
来源：http://fkv.sjlbkw.cn

(double) a / b
来源：http://vic.quarkkingdee.top

[S16] C：位操作置位
来源：http://krx.yj20258.top

x |= (1 << 3);
来源：http://bjt.quarkkingdee.top

[S17] C：安全拼接字符串
来源：http://jgk.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vgp.zhengqikj.top

[S18] C：命令行参数
来源：http://ebj.tanke756.top


<!-- 参考信息 -->