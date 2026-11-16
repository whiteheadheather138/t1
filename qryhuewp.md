代发 wailian999

[Q61] 移动平均
来源：http://bxo.jyoumei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lwu.wangshuangyany.cn

[Q62] 分组占比
来源：http://yyd.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qmb.sweek.top

[Q63] 开启事务
来源：http://cis.guowangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lyw.aibaodan.cn

[Q64] 提交事务
来源：http://zkz.bbcook.cn

COMMIT;
来源：http://rnc.zhixingplan.top

[Q65] 回滚事务
来源：http://tok.wangshuangyany.cn

ROLLBACK;
来源：http://fpz.cucudq.cn

[Q66] 行锁查询
来源：http://neb.xuanzx.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://koz.gogol.net.cn

[Q67] 设置隔离级别
来源：http://pmr.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kzm.shzxlz.cn

[Q68] 保存点
来源：http://wvh.fehbvm.com

SAVEPOINT sp1;
来源：http://uhp.daxiang520.top

ROLLBACK TO sp1;
来源：http://kxg.yj20258888.top

[Q69] 查看执行计划
来源：http://fxn.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pln.xuetiantiany.cn

[Q70] 更新统计信息
来源：http://upg.daxiang520.top

ANALYZE TABLE users;
来源：http://cgl.jiagoushi.top

[Q71] 查看建表语句
来源：http://mhc.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dpy.cucudq.cn

[Q72] 查看索引
来源：http://odm.cheryme.top

SHOW INDEX FROM users;
来源：http://lzm.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://smn.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xzy.snrcjt.cn

[Q74] 强制使用索引
来源：http://trc.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dag.zycfv.cn

[Q75] 日期格式化
来源：http://jew.jinyuanbaomall.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xay.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ojd.chenlongwang.top

[Q76] 按天统计
来源：http://qek.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zyh.ctjpmb.com

[Q77] 时间加减
来源：http://dzw.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://brp.ctjpmb.com

[Q78] 当前时间
来源：http://fsp.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://csn.hywenlv.cn

[Q79] 字符串拼接
来源：http://bok.sxryk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hwf.shanyushiyangtech.top

[Q80] 字符串截取
来源：http://duu.dashuyun.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bse.c1oappe.top

[Q81] 字符串替换
来源：http://fic.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://buu.shangyingyoupin.top

[Q82] 字符长度与字节长度
来源：http://eij.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dze.tianlin.xyz

[Q83] 大小写转换
来源：http://cdl.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yzh.birdmap.top

[Q84] 去除首尾空格
来源：http://aeu.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://yqo.svipenyu.cn

[Q85] 数值取整
来源：http://zai.snrcjt.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://coc.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://afk.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nmv.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://cwe.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://num.zdqjudy.top

[Q88] 行转列（条件聚合）
来源：http://zle.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://usl.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iad.hywenlv.cn

[Q89] 判断表是否存在
来源：http://cby.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fop.tarul.cn

[Q90] 生成序号列
来源：http://fuu.zhongyouzk.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yxv.xingfuxueyuan.xyz

================================================================================
来源：http://xhv.xziqi.cn

R. Bash 专题
来源：http://otd.sufxvd.cn

================================================================================
来源：http://avc.yj20258.top

[R01] shebang 与严格模式
来源：http://yfq.chenlongwang.top

#!/usr/bin/env bash
来源：http://qle.jinghuilouyu.cn

set -euo pipefail
来源：http://yrw.yuxming.cn

[R02] 变量赋值与使用
来源：http://pyb.hammf.cn

name="Tom"; echo "$name"
来源：http://sub.sweek.top

[R03] 只读变量
来源：http://gac.yj20258888.top

readonly PI=3.14
来源：http://rop.zhoulong.xyz

[R04] 位置参数
来源：http://dyr.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ngv.cheryme.top

[R05] 参数默认值
来源：http://rmy.chenlongwang.top

name="${1:-default}"
来源：http://bra.gzhubu.top

[R06] 判断命令是否存在
来源：http://kmi.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wgs.zdqjudy.top

[R07] if 判断文件
来源：http://nps.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fxo.ydjk.org.cn

[R08] 数值比较
来源：http://ezd.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hod.xylfe.cn

[R09] 字符串比较
来源：http://qot.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://htf.dashuyun.cn

[R10] 正则匹配
来源：http://uhf.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jdl.wangdashe.top

[R11] case 多分支
来源：http://hdt.fehbvm.com

case "$1" in
来源：http://mfo.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://hou.dashuyun.cn

stop)  echo "停止" ;;
来源：http://ncm.guannengcc.top

*)     echo "未知命令" ;;
来源：http://dsn.tian-w.cn

esac
来源：http://ytb.yj202588.top

[R12] for 遍历文件
来源：http://jhv.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://mxd.hnxiangtu.top

[R13] for 计数循环
来源：http://xyt.52xcode.cn

for i in {1..10}; do echo "$i"; done
来源：http://kza.hesvh.cn

[R14] C 风格 for
来源：http://mtk.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lyn.cheryme.top

[R15] while 逐行读文件
来源：http://xgg.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mqj.jinghuilouyu.cn

[R16] until 等待条件
来源：http://hls.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rsl.ivvv.top

[R17] 数组定义与取值
来源：http://vyn.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://hym.tian-w.cn

[R18] 遍历数组
来源：http://mwk.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bdc.cucudq.cn

[R19] 数组长度
来源：http://giv.ehwqpu.com

echo "${#arr[@]}"
来源：http://oie.shanyushiyangtech.top

[R20] 关联数组（字典）
来源：http://qro.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pkx.sweek.top

[R21] 字符串长度
来源：http://irm.xinyue.icu

echo "${#s}"
来源：http://dcd.shzxlz.cn

[R22] 截取子串
来源：http://shl.bjfxy.top

echo "${s:0:5}"
来源：http://jnj.pycfn.com

[R23] 字符串替换
来源：http://wgw.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tvx.dashuyun.cn

[R24] 大小写转换
来源：http://nxb.0kj1m.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bvu.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://fns.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lcn.ivvv.top

[R26] 命令替换
来源：http://hoy.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://goy.zycfv.cn

[R27] 算术展开
来源：http://npo.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://jzc.yuxming.cn

[R28] 浮点运算
来源：http://xgi.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://kja.sysykeji.top

[R29] 定义函数
来源：http://lbq.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mos.birdmap.top

[R30] 函数返回状态码
来源：http://tnl.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://gwb.snrcjt.cn

[R31] 局部变量
来源：http://gns.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://bvw.yj20258888.top

[R32] 参数个数校验
来源：http://tar.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xoz.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://ryn.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hza.jiagoushi.top

[R34] 退出时清理
来源：http://pwm.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fjo.bjfxy.top

[R35] 后台执行并等待
来源：http://qrw.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wae.ehwqpu.com

[R36] 并发执行多个任务
来源：http://rxv.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://osj.jlsjyb.cn

[R37] 把输出赋给变量
来源：http://gyp.epnwcf.com

files=$(ls -1)
来源：http://voy.shuidangran.top

[R38] 管道串联
来源：http://fxg.0kj1m.cn

cat a.txt | grep -i error | wc -l
来源：http://khe.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://eic.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://pob.xziqi.cn

[R40] 追加写日志
来源：http://kob.wangshuangyany.cn

echo "log" >> out.log
来源：http://ihj.daxiang520.top

[R41] 丢弃输出
来源：http://zuj.tian-w.cn

cmd >/dev/null 2>&1
来源：http://nnm.hesvh.cn

[R42] 输入重定向
来源：http://yaj.yuanzhike.top

wc -l < a.txt
来源：http://lmn.jinqigfzy.top

[R43] 按名字查找文件
来源：http://tui.yuxming.cn

find . -name "*.log" -type f
来源：http://usy.daria6918.cn

[R44] 按修改时间查找
来源：http://vhb.aibaodan.cn

find . -mtime -7 -type f
来源：http://syw.9152youxi.cn

[R45] 批量删除
来源：http://lba.tanke756.top

find . -name "*.tmp" -delete
来源：http://dsy.havefunace.top

[R46] 递归替换文件内容
来源：http://cat.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hoj.redwolf501.top

[R47] sed 单行替换
来源：http://uzn.daxiang520.top

sed -i 's/foo/bar/g' a.txt
来源：http://xuk.ywan-chungtsiang.top

[R48] awk 取指定列
来源：http://sbg.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://rqj.zdbjq.cn

[R49] awk 带条件
来源：http://zwh.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xof.shuidangran.top

[R50] awk 求和
来源：http://lpz.52xcode.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sso.aizwys.cn

[R51] 排序去重取前几
来源：http://tnc.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fho.gogol.net.cn

[R52] 统计行数
来源：http://ztu.52xcode.cn

wc -l a.txt
来源：http://nbs.tian-w.cn

[R53] 查看文件头与实时尾
来源：http://ett.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ino.jlsjyb.cn

[R54] 比较两个文件
来源：http://zqn.wangshuangyany.cn

diff a.txt b.txt
来源：http://yne.yuxming.cn

[R55] 压缩与解压
来源：http://alh.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gec.gzhubu.top

[R56] 远程拷贝
来源：http://vnc.c1oappe.top

scp file user@host:/path/
来源：http://jbi.yfazqb.com

[R57] 远程执行命令
来源：http://vpp.xuanzx.com

ssh user@host 'uptime'
来源：http://txo.9152youxi.cn

[R58] 下载文件
来源：http://nfh.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gbo.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://yro.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zib.tian-w.cn

[R60] 只看 HTTP 状态码
来源：http://qwu.bjfxy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hok.havefunace.top

[R61] 磁盘占用
来源：http://wnm.cucudq.cn

df -h;  du -sh *
来源：http://eoq.sweek.top

[R62] 找最占空间的文件
来源：http://gaw.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://erp.jqgufenzy.top

[R63] 内存与进程
来源：http://lpl.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://shp.zdbjq.cn

[R64] 结束进程
来源：http://dae.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://ejr.fktsv.cn

[R65] 查看端口占用
来源：http://wkh.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://alg.ywan-chungtsiang.top

[R66] 定时任务
来源：http://npo.jlsjyb.cn

crontab -e;  crontab -l
来源：http://ryf.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://efe.c1oappe.top

openssl rand -hex 16
来源：http://mfq.ehwqpu.com

[R68] 计算文件校验值
来源：http://els.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://fnb.chenzaomai.com

[R69] 生成随机密码
来源：http://fdg.sysykeji.top

head -c 16 /dev/urandom | base64
来源：http://nrg.tianlin.xyz

[R70] 时间戳与互转
来源：http://edf.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://vos.snrcjt.cn

[R71] 日期格式化
来源：http://xhe.yongpay.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pbf.yj202588.top

[R72] 等待端口就绪
来源：http://gpe.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qrh.tanke756.top

[R73] 分割大日志
来源：http://umf.hysaishi.cn

split -l 1000 big.log part_
来源：http://rwn.wangdashe.top

[R74] 批量重命名
来源：http://hue.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gja.zhiwuduotai.top

[R75] 导出环境变量
来源：http://xqp.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://our.snrcjt.cn

[R76] 使用临时文件
来源：http://sbi.jqgfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ffo.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://szg.havefunace.top

read -rp "请输入: " ans
来源：http://pos.chenjidiqi.icu

[R78] 交互式菜单
来源：http://acj.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lzw.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://jyp.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yhc.daria6918.cn

[R80] 查看脚本执行耗时
来源：http://gpf.tian-w.cn

time ./run.sh
来源：http://fto.gogol.net.cn

================================================================================
来源：http://mvx.wangshuangyany.cn

S. C / C++ 专题
来源：http://fcn.ydzc1.top

================================================================================
来源：http://zhq.kuanghao11.cn

[S01] C：Hello World
来源：http://xlt.andypj.xyz

#include <stdio.h>
来源：http://ycf.aibaodan.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wqh.hesvh.cn

[S02] C：变量与格式化输出
来源：http://usk.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://elb.aizwys.cn

[S03] C：读入整数
来源：http://jim.tian-w.cn

int x; scanf("%d", &x);
来源：http://yqa.birdmap.top

[S04] C：字符串复制
来源：http://bsp.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://eab.zhiwuduotai.top

[S05] C：字符串长度
来源：http://vbm.ppjwa.cn

strlen(s)
来源：http://xhn.xingfuxueyuan.xyz

[S06] C：字符串比较
来源：http://wcq.xziqi.cn

strcmp(a, b) == 0
来源：http://xxy.tarul.cn

[S07] C：数组遍历求和
来源：http://eqe.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://axq.pycfn.com

[S08] C：动态内存分配与释放
来源：http://rgo.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rvi.hnqzz.top

[S09] C：结构体定义与初始化
来源：http://vvj.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ihi.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://hmt.yfazqb.com

int *p = &a;  *p = 5;
来源：http://ckb.ydzc1.top

[S11] C：逐行读文件
来源：http://gqz.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://qlt.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lnj.sysykeji.top

fclose(f);
来源：http://ooz.zdqjudy.top

[S12] C：写文件
来源：http://sts.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://azv.sysykeji.top

[S13] C：宏定义
来源：http://bkx.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ncl.yuxming.cn

[S14] C：枚举
来源：http://owq.jlsjyb.cn

enum Color { RED, GREEN, BLUE };
来源：http://rps.jinghuilouyu.cn

[S15] C：类型转换
来源：http://sst.fzhhl.top

(double) a / b
来源：http://sai.haohaochexian.top

[S16] C：位操作置位
来源：http://wrq.xuetiantiany.cn

x |= (1 << 3);
来源：http://msm.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://lye.yueranfly.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://faw.jinghuilouyu.cn

[S18] C：命令行参数
来源：http://aet.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://njo.ivvv.top

[S19] C：快速排序
来源：http://waf.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://qmp.cqqwz.cn

[S20] C：二分查找
来源：http://xgk.daxiang520.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vtj.shanyushiyangkeji.top

[S21] C：字符类别判断
来源：http://avq.zdbjq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kgk.ppjwa.cn

[S22] C：字符串转数字
来源：http://yht.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://urm.hnqzz.top

[S23] C：随机数
来源：http://ypv.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mss.tarul.cn

[S24] C：获取本地时间
来源：http://ilz.gaohongyu789.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://moe.bbcook.cn

[S25] C：内存拷贝
来源：http://opv.dashuyun.cn

memcpy(dst, src, n);
来源：http://ugs.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://ggv.jinghuilouyu.cn

memset(a, 0, sizeof a);
来源：http://ziz.nwbrower.top

[S27] C：定义常量
来源：http://rib.ivvv.top

const double PI = 3.14159;
来源：http://yxo.guannengcc.top

[S28] C：静态变量
来源：http://bqd.xinyue.icu

static int counter = 0;
来源：http://acs.yvedp.cn

[S29] C：变参函数
来源：http://bdl.ybcxt.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gxx.aizwys.cn

[S30] C：头文件保护
来源：http://fpp.zhijiandao.cn

#ifndef X_H
来源：http://pzf.shanyushiyangtech.top

#define X_H
来源：http://kqq.zdbjq.cn

#endif
来源：http://rnj.ybcxt.top

[S31] C++：Hello World
来源：http://fwx.xingfuxueyuan.xyz


<!-- 参考信息 -->