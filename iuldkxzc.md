代发 wailian999

[Q65] 回滚事务
来源：http://ljs.ywan-chungtsiang.top

ROLLBACK;
来源：http://obb.sysykeji.top

[Q66] 行锁查询
来源：http://gpw.shanyushiyangtech.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xnc.sysykeji.top

[Q67] 设置隔离级别
来源：http://kod.tanke756.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mnz.yfazqb.com

[Q68] 保存点
来源：http://wnq.yuxming.cn

SAVEPOINT sp1;
来源：http://pdx.guannengcc.top

ROLLBACK TO sp1;
来源：http://gwd.yfazqb.com

[Q69] 查看执行计划
来源：http://zvj.zhijiandao.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yrq.cqqwz.cn

[Q70] 更新统计信息
来源：http://nfn.haohaochexian.top

ANALYZE TABLE users;
来源：http://bon.tarul.cn

[Q71] 查看建表语句
来源：http://lvj.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pmr.hammf.cn

[Q72] 查看索引
来源：http://vcd.ctjpmb.com

SHOW INDEX FROM users;
来源：http://gdt.yj202588.top

[Q73] 查看表状态
来源：http://oph.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://mmm.yuxming.cn

[Q74] 强制使用索引
来源：http://jvq.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uiq.jqgfzy.top

[Q75] 日期格式化
来源：http://cfr.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dsu.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wvk.chenlongwang.top

[Q76] 按天统计
来源：http://xcg.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xtm.shangyingyoupin.top

[Q77] 时间加减
来源：http://icy.xuanzx.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uts.feifeiyinyue.top

[Q78] 当前时间
来源：http://ncq.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mtd.nanxinkj.top

[Q79] 字符串拼接
来源：http://zba.bjfxy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cny.nanxuanxn.top

[Q80] 字符串截取
来源：http://wsp.yuxming.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ngc.tian-w.cn

[Q81] 字符串替换
来源：http://cwf.xingfuxueyuan.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bqm.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://iav.fengsongda.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yjn.redwolf501.top

[Q83] 大小写转换
来源：http://cdo.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mao.mhx1999.top

[Q84] 去除首尾空格
来源：http://hmb.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://oec.aibaodan.cn

[Q85] 数值取整
来源：http://ipl.yj20258.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dbs.fengsongda.top

[Q86] 读取 JSON 字段
来源：http://cku.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kbp.xinyue.icu

[Q87] JSON 字段做条件
来源：http://psf.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zkw.0kj1m.cn

[Q88] 行转列（条件聚合）
来源：http://sfp.c1oappe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://khm.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kqn.daxiang520.top

[Q89] 判断表是否存在
来源：http://wdm.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mik.uphjek.com

[Q90] 生成序号列
来源：http://zgr.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kkr.ivvv.top

================================================================================
来源：http://giz.tian-w.cn

R. Bash 专题
来源：http://nnf.zycfv.cn

================================================================================
来源：http://quq.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://mre.zdqjudy.top

#!/usr/bin/env bash
来源：http://cni.birdmap.top

set -euo pipefail
来源：http://axc.fehbvm.com

[R02] 变量赋值与使用
来源：http://ino.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://tsz.aizwys.cn

[R03] 只读变量
来源：http://cyg.gogol.net.cn

readonly PI=3.14
来源：http://znw.hongshengwenyu.top

[R04] 位置参数
来源：http://zvi.yanxiufei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://spk.nanxinkj.top

[R05] 参数默认值
来源：http://lik.shanyushiyangtech.top

name="${1:-default}"
来源：http://lzq.yangfankeji.com

[R06] 判断命令是否存在
来源：http://anq.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://crr.andypj.xyz

[R07] if 判断文件
来源：http://twq.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ewa.zdbjq.cn

[R08] 数值比较
来源：http://nov.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://epx.sysykeji.top

[R09] 字符串比较
来源：http://xrs.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://exu.yvedp.cn

[R10] 正则匹配
来源：http://jju.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jvn.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://wcv.daxiang520.top

case "$1" in
来源：http://bsk.hnqzz.top

start) echo "启动" ;;
来源：http://zmb.ehwqpu.com

stop)  echo "停止" ;;
来源：http://eed.xuanzx.com

*)     echo "未知命令" ;;
来源：http://oaj.yuxming.cn

esac
来源：http://yut.fehbvm.com

[R12] for 遍历文件
来源：http://jks.xylfe.cn

for f in *.txt; do echo "$f"; done
来源：http://goy.yvedp.cn

[R13] for 计数循环
来源：http://mmd.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://gkl.sjlbkw.cn

[R14] C 风格 for
来源：http://yuk.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fof.gzhubu.top

[R15] while 逐行读文件
来源：http://okg.jiagoushi.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hef.chenjidiqi.icu

[R16] until 等待条件
来源：http://oid.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qmy.aizwys.cn

[R17] 数组定义与取值
来源：http://ftf.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://gdg.sjlbkw.cn

[R18] 遍历数组
来源：http://mxw.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://exs.cdnleiting.top

[R19] 数组长度
来源：http://ijz.quarkkingdee.top

echo "${#arr[@]}"
来源：http://izl.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://kzv.zhaomingkeji.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bna.xuetiantiany.cn

[R21] 字符串长度
来源：http://lkn.jinqigufen.top

echo "${#s}"
来源：http://gtp.meibo888.top

[R22] 截取子串
来源：http://rzd.nwbrower.top

echo "${s:0:5}"
来源：http://kqc.chenlongwang.top

[R23] 字符串替换
来源：http://aif.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zpd.hfpthk.cn

[R24] 大小写转换
来源：http://kpa.gaohongyu789.top

echo "${s^^}"; echo "${s,,}"
来源：http://hxg.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://lsi.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zcx.gzhubu.top

[R26] 命令替换
来源：http://adl.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://rqg.yfazqb.com

[R27] 算术展开
来源：http://dnz.xinyue.icu

echo $((1 + 2 * 3))
来源：http://nps.zycfv.cn

[R28] 浮点运算
来源：http://fxd.birdmap.top

echo "scale=2; 10/3" | bc
来源：http://swg.zhixingplan.top

[R29] 定义函数
来源：http://tmh.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qql.chenlongwang.top

[R30] 函数返回状态码
来源：http://ctx.hammf.cn

f() { return 0; }; f || echo "失败了"
来源：http://lan.pengpengdd.cyou

[R31] 局部变量
来源：http://gcp.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://iak.zhijiandao.cn

[R32] 参数个数校验
来源：http://nmr.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hyk.yj202588.top

[R33] 捕获错误并提示行号
来源：http://arw.gzhubu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wxd.shzxlz.cn

[R34] 退出时清理
来源：http://bdo.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tqi.yanxiufei.cn

[R35] 后台执行并等待
来源：http://rvs.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oja.sjlbkw.cn

[R36] 并发执行多个任务
来源：http://sex.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iuk.havefunace.top

[R37] 把输出赋给变量
来源：http://wfn.fengsongda.top

files=$(ls -1)
来源：http://pdv.jlsjyb.cn

[R38] 管道串联
来源：http://ywb.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://xml.jqgfzy.top

[R39] 重定向标准输出与错误
来源：http://evq.c1oappe.top

cmd > out.log 2>&1
来源：http://vun.ivvv.top

[R40] 追加写日志
来源：http://spy.haohaochexian.top

echo "log" >> out.log
来源：http://vbr.xinyue.icu

[R41] 丢弃输出
来源：http://fwj.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://wmf.jinqigfzy.top

[R42] 输入重定向
来源：http://ozr.shuidangran.top

wc -l < a.txt
来源：http://vku.jqgufenzy.top

[R43] 按名字查找文件
来源：http://tgo.hywenlv.cn

find . -name "*.log" -type f
来源：http://kzk.zhongyouzk.top

[R44] 按修改时间查找
来源：http://kfg.cqqwz.cn

find . -mtime -7 -type f
来源：http://fkt.shanyushiyangtech.top

[R45] 批量删除
来源：http://ewm.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://zco.yvedp.cn

[R46] 递归替换文件内容
来源：http://tmz.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xrb.ydzc1.top

[R47] sed 单行替换
来源：http://ezf.yueranfly.top

sed -i 's/foo/bar/g' a.txt
来源：http://hwf.yuanzhike.top

[R48] awk 取指定列
来源：http://xbe.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://oid.sufxvd.cn

[R49] awk 带条件
来源：http://jbf.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ukn.sysykeji.top

[R50] awk 求和
来源：http://oys.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ejn.zhijiandao.cn

[R51] 排序去重取前几
来源：http://qrz.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zhc.nanxinkj.top

[R52] 统计行数
来源：http://tyq.jinyuanbaomall.cn

wc -l a.txt
来源：http://sra.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://xyn.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pkm.uphjek.com

[R54] 比较两个文件
来源：http://cmo.zycfv.cn

diff a.txt b.txt
来源：http://xsb.sysykeji.top

[R55] 压缩与解压
来源：http://sfe.ppjwa.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wpl.shuidangran.top

[R56] 远程拷贝
来源：http://zxx.guannengcc.top

scp file user@host:/path/
来源：http://grq.yuanzhike.top

[R57] 远程执行命令
来源：http://stm.hfpthk.cn

ssh user@host 'uptime'
来源：http://pxv.zdqjudy.top

[R58] 下载文件
来源：http://spb.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://knz.xylfe.cn

[R59] 发 POST JSON
来源：http://txi.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xzk.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://zbt.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xbb.9152youxi.cn

[R61] 磁盘占用
来源：http://cnf.0kj1m.cn

df -h;  du -sh *
来源：http://aik.aizwys.cn

[R62] 找最占空间的文件
来源：http://osk.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://quz.yj202588.top

[R63] 内存与进程
来源：http://pad.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://nup.uphjek.com

[R64] 结束进程
来源：http://slq.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://ooz.tanke756.top

[R65] 查看端口占用
来源：http://vln.smart0.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fpa.jinqigufen.top

[R66] 定时任务
来源：http://jcq.quarkkingdee.top

crontab -e;  crontab -l
来源：http://pct.fanxiaobao.xyz

[R67] 生成随机十六进制串
来源：http://nkf.mhx1999.top

openssl rand -hex 16
来源：http://ecd.yj202588.top

[R68] 计算文件校验值
来源：http://hks.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://ngk.svipenyu.cn

[R69] 生成随机密码
来源：http://nyu.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://lpc.hnqzz.top

[R70] 时间戳与互转
来源：http://lcw.fehbvm.com

date +%s;  date -d @1700000000
来源：http://gum.yfazqb.com

[R71] 日期格式化
来源：http://yco.hnxiangtu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vrh.haohaochexian.top

[R72] 等待端口就绪
来源：http://koj.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dqn.ydzc1.top

[R73] 分割大日志
来源：http://bes.zycfv.cn

split -l 1000 big.log part_
来源：http://lez.sxryk.cn

[R74] 批量重命名
来源：http://gsb.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yza.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://kvf.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://qhv.yueranfly.top

[R76] 使用临时文件
来源：http://gmy.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yfs.zhengqikj.top

[R77] 读取用户输入
来源：http://bea.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://aoz.cucudq.cn

[R78] 交互式菜单
来源：http://azb.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fex.nwbrower.top

[R79] 解析命令行选项
来源：http://jat.epnwcf.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jxl.uphjek.com

[R80] 查看脚本执行耗时
来源：http://cec.daxiang520.top

time ./run.sh
来源：http://qcn.zhoulong.xyz

================================================================================
来源：http://bry.mhx1999.top

S. C / C++ 专题
来源：http://mme.aibaodan.cn

================================================================================
来源：http://gns.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://osm.xuanzx.com

#include <stdio.h>
来源：http://crr.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cyk.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://tks.0kj1m.cn

int a = 10; printf("%d\n", a);
来源：http://yqt.smart0.xyz

[S03] C：读入整数
来源：http://smr.jinghuilouyu.cn

int x; scanf("%d", &x);
来源：http://djs.havefunace.top

[S04] C：字符串复制
来源：http://bgm.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mmc.pycfn.com

[S05] C：字符串长度
来源：http://ixz.aibaodan.cn

strlen(s)
来源：http://jlx.ivvv.top

[S06] C：字符串比较
来源：http://otx.ydzc1.top

strcmp(a, b) == 0
来源：http://zjz.sweek.top

[S07] C：数组遍历求和
来源：http://ibp.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dhh.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://gbl.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tlj.yuxming.cn

[S09] C：结构体定义与初始化
来源：http://afv.daxiang520.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ipj.fktsv.cn

[S10] C：指针与解引用
来源：http://edo.52xcode.cn

int *p = &a;  *p = 5;
来源：http://sas.tarul.cn

[S11] C：逐行读文件
来源：http://jhu.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://mpz.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kfz.zhongyouzk.top

fclose(f);
来源：http://apu.havefunace.top

[S12] C：写文件
来源：http://cod.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pwu.yvedp.cn

[S13] C：宏定义
来源：http://nms.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nsm.pycfn.com

[S14] C：枚举
来源：http://cjg.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://tqb.ppjwa.cn

[S15] C：类型转换
来源：http://fxo.mhx1999.top

(double) a / b
来源：http://ptu.52xcode.cn

[S16] C：位操作置位
来源：http://vkk.zhijiandao.cn

x |= (1 << 3);
来源：http://dcd.jianghu66.top

[S17] C：安全拼接字符串
来源：http://uob.yfazqb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dgn.smart0.xyz

[S18] C：命令行参数
来源：http://rgz.cdnleiting.top

int main(int argc, char **argv)
来源：http://vot.tianlin.xyz

[S19] C：快速排序
来源：http://qcz.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qfl.smart0.xyz

[S20] C：二分查找
来源：http://qcd.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qer.havefunace.top

[S21] C：字符类别判断
来源：http://hlp.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zri.quarkkingdee.top

[S22] C：字符串转数字
来源：http://aaq.zhaomingkeji.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://abw.xylfe.cn

[S23] C：随机数
来源：http://qum.hesvh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wgb.zhijiandao.cn

[S24] C：获取本地时间
来源：http://qjx.yfazqb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mhg.daria6918.cn

[S25] C：内存拷贝
来源：http://oex.zycfv.cn

memcpy(dst, src, n);
来源：http://rwn.yanxiufei.cn

[S26] C：内存清零
来源：http://npm.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://jei.wangshuangyany.cn

[S27] C：定义常量
来源：http://zbb.shangyingyoupin.top

const double PI = 3.14159;
来源：http://ppc.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://woq.gaohongyu789.top

static int counter = 0;
来源：http://vkw.jianghu66.top

[S29] C：变参函数
来源：http://vye.xuetiantiany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sxa.jqgufenzy.top

[S30] C：头文件保护
来源：http://cvm.yj20258.top

#ifndef X_H
来源：http://oje.xinyue.icu

#define X_H
来源：http://tyk.sweek.top

#endif
来源：http://mrw.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://vig.fzhhl.top

#include <iostream>
来源：http://hzn.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://gsd.andypj.xyz

[S32] C++：字符串
来源：http://wak.9152youxi.cn

std::string s = "hi";  s += "!";
来源：http://rrg.snrcjt.cn

[S33] C++：vector 增删
来源：http://pbs.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wms.mhx1999.top

[S34] C++：遍历 vector
来源：http://pqo.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://tvj.316326.xyz


<!-- 参考信息 -->