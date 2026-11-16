代发 wailian999

ANALYZE TABLE users;
来源：http://gfx.hnqzz.top

[Q71] 查看建表语句
来源：http://lsc.hnxiangtu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ptr.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://yhw.nanxinkj.top

SHOW INDEX FROM users;
来源：http://dyx.ydjk.org.cn

[Q73] 查看表状态
来源：http://lgx.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://qkn.chenlongwang.top

[Q74] 强制使用索引
来源：http://ksj.52xcode.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iyn.kuanghao11.cn

[Q75] 日期格式化
来源：http://ans.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lct.havefunace.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://owf.jinghuilouyu.cn

[Q76] 按天统计
来源：http://jhi.epnwcf.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bhg.feifeiyinyue.top

[Q77] 时间加减
来源：http://kfw.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rzk.ctjpmb.com

[Q78] 当前时间
来源：http://umt.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yse.hesvh.cn

[Q79] 字符串拼接
来源：http://ury.kuanghao11.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ppb.haohaochexian.top

[Q80] 字符串截取
来源：http://vgd.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mnr.hysaishi.cn

[Q81] 字符串替换
来源：http://ndk.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hcm.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://cmv.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://djv.redwolf501.top

[Q83] 大小写转换
来源：http://aku.tian-w.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nzm.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://uql.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://iqd.yj20258.top

[Q85] 数值取整
来源：http://vwr.zhiwuduotai.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tjb.nwbrower.top

[Q86] 读取 JSON 字段
来源：http://rqp.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bay.yj20258888.top

[Q87] JSON 字段做条件
来源：http://mwp.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kuk.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://xaf.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xot.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jro.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://plb.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nxk.ivvv.top

[Q90] 生成序号列
来源：http://gty.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qai.shanyushiyangtech.top

================================================================================
来源：http://kfx.zdqjudy.top

R. Bash 专题
来源：http://yut.shzxlz.cn

================================================================================
来源：http://pgt.jyoumei.cn

[R01] shebang 与严格模式
来源：http://qap.iojbl.cn

#!/usr/bin/env bash
来源：http://uas.fzhhl.top

set -euo pipefail
来源：http://ahl.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://drb.xinyue.icu

name="Tom"; echo "$name"
来源：http://aat.jqgfzy.top

[R03] 只读变量
来源：http://nxw.yj20258888.top

readonly PI=3.14
来源：http://zqh.gogol.net.cn

[R04] 位置参数
来源：http://keg.bjfxy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xie.bjfxy.top

[R05] 参数默认值
来源：http://mqg.ctjpmb.com

name="${1:-default}"
来源：http://wpc.zhengqikj.top

[R06] 判断命令是否存在
来源：http://gae.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tqd.sweek.top

[R07] if 判断文件
来源：http://ncn.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yyg.vehdjk.com

[R08] 数值比较
来源：http://wux.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://bjf.hysaishi.cn

[R09] 字符串比较
来源：http://uhk.fktsv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qbf.cdnleiting.top

[R10] 正则匹配
来源：http://mmi.chenjidiqi.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://krv.yuanzhike.top

[R11] case 多分支
来源：http://oee.pengpengdd.cyou

case "$1" in
来源：http://wyr.jianghu66.top

start) echo "启动" ;;
来源：http://xbb.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://yub.xylfe.cn

*)     echo "未知命令" ;;
来源：http://iyh.ybcxt.top

esac
来源：http://mwz.hesvh.cn

[R12] for 遍历文件
来源：http://vgh.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://fwy.havefunace.top

[R13] for 计数循环
来源：http://lau.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://paf.xuanzx.com

[R14] C 风格 for
来源：http://qpg.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kuo.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://eng.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xur.yueranfly.top

[R16] until 等待条件
来源：http://kwr.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://trc.zhiwuduotai.top

[R17] 数组定义与取值
来源：http://veo.daria6918.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yac.sjlbkw.cn

[R18] 遍历数组
来源：http://dwq.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dxj.sjlbkw.cn

[R19] 数组长度
来源：http://qwe.yanxiufei.cn

echo "${#arr[@]}"
来源：http://oqv.fanxiaobao.xyz

[R20] 关联数组（字典）
来源：http://upc.hysaishi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://njn.dashuyun.cn

[R21] 字符串长度
来源：http://xvk.yanxiufei.cn

echo "${#s}"
来源：http://zhe.dashuyun.cn

[R22] 截取子串
来源：http://hdl.havefunace.top

echo "${s:0:5}"
来源：http://juk.birdmap.top

[R23] 字符串替换
来源：http://ymm.guannengcc.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vlz.gzhubu.top

[R24] 大小写转换
来源：http://yav.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://juk.0kj1m.cn

[R25] 去后缀 / 去前缀
来源：http://fvm.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://vdf.chenlongwang.top

[R26] 命令替换
来源：http://wyg.zdbjq.cn

now=$(date +%F); echo "$now"
来源：http://idj.zdqjudy.top

[R27] 算术展开
来源：http://vnq.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://gvc.epnwcf.com

[R28] 浮点运算
来源：http://lmb.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://iii.sxryk.cn

[R29] 定义函数
来源：http://wzz.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://afc.gaohongyu789.top

[R30] 函数返回状态码
来源：http://bnq.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://kdw.jqgufenzy.top

[R31] 局部变量
来源：http://xov.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://wqu.fehbvm.com

[R32] 参数个数校验
来源：http://wtz.mhx1999.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hhr.nanxinkj.top

[R33] 捕获错误并提示行号
来源：http://ybx.nwbrower.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://duk.hywenlv.cn

[R34] 退出时清理
来源：http://wfn.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sag.hnxiangtu.top

[R35] 后台执行并等待
来源：http://qqj.yvedp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qnp.fanxiaobao.xyz

[R36] 并发执行多个任务
来源：http://vug.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://izj.nanxinkj.top

[R37] 把输出赋给变量
来源：http://rnk.haohaochexian.top

files=$(ls -1)
来源：http://aie.daria6918.cn

[R38] 管道串联
来源：http://per.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://cqz.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://ezr.shzxlz.cn

cmd > out.log 2>&1
来源：http://qgd.fanxiaobao.xyz

[R40] 追加写日志
来源：http://gry.shangyingyoupin.top

echo "log" >> out.log
来源：http://him.wangshuangyany.cn

[R41] 丢弃输出
来源：http://tpz.sxryk.cn

cmd >/dev/null 2>&1
来源：http://fij.yj20258.top

[R42] 输入重定向
来源：http://sru.yj20258.top

wc -l < a.txt
来源：http://zet.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://wfn.feifeiyinyue.top

find . -name "*.log" -type f
来源：http://yth.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://tsw.hysaishi.cn

find . -mtime -7 -type f
来源：http://rwf.316326.xyz

[R45] 批量删除
来源：http://unl.iojbl.cn

find . -name "*.tmp" -delete
来源：http://gtl.zycfv.cn

[R46] 递归替换文件内容
来源：http://qjt.yuxming.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vex.redwolf501.top

[R47] sed 单行替换
来源：http://xiq.pengpengdd.cyou

sed -i 's/foo/bar/g' a.txt
来源：http://dra.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://jfp.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://xxv.ydjk.org.cn

[R49] awk 带条件
来源：http://rcp.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://goy.fengsongda.top

[R50] awk 求和
来源：http://cej.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://xyx.yuxming.cn

[R51] 排序去重取前几
来源：http://jjh.52xcode.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pan.cashguo.top

[R52] 统计行数
来源：http://bkz.tarul.cn

wc -l a.txt
来源：http://lib.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://xoo.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kxj.jyoumei.cn

[R54] 比较两个文件
来源：http://mjo.vqdsnc.cn

diff a.txt b.txt
来源：http://qdh.zhengqikj.top

[R55] 压缩与解压
来源：http://gxf.yj202588.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zec.zdbjq.cn

[R56] 远程拷贝
来源：http://hws.epnwcf.com

scp file user@host:/path/
来源：http://rjw.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://bbd.jqgfzy.top

ssh user@host 'uptime'
来源：http://rlo.chenjidiqi.icu

[R58] 下载文件
来源：http://omk.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uqf.yj202588.top

[R59] 发 POST JSON
来源：http://ggq.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://duf.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://uce.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nix.gogol.net.cn

[R61] 磁盘占用
来源：http://rho.hcnkem.com

df -h;  du -sh *
来源：http://nlm.yonumen.top

[R62] 找最占空间的文件
来源：http://ipc.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://xkg.bbcook.cn

[R63] 内存与进程
来源：http://iuy.hammf.cn

free -h;  ps aux | grep nginx
来源：http://imn.dianchejie.cn

[R64] 结束进程
来源：http://etw.svipenyu.cn

kill -9 $(pgrep -f app.py)
来源：http://qvm.andypj.xyz

[R65] 查看端口占用
来源：http://rim.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://slb.tarul.cn

[R66] 定时任务
来源：http://agi.dashuyun.cn

crontab -e;  crontab -l
来源：http://ekd.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://yzp.hnxiangtu.top

openssl rand -hex 16
来源：http://trz.jinqigufen.top

[R68] 计算文件校验值
来源：http://pdh.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uls.yanxiufei.cn

[R69] 生成随机密码
来源：http://rel.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://xey.mhx1999.top

[R70] 时间戳与互转
来源：http://bob.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://wey.guannengcc.top

[R71] 日期格式化
来源：http://edj.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://iah.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://odc.chenzaomai.com

until nc -z localhost 3306; do sleep 1; done
来源：http://sfi.nwbrower.top

[R73] 分割大日志
来源：http://oud.hnxiangtu.top

split -l 1000 big.log part_
来源：http://pti.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://hfp.fktsv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jyz.yangfankeji.com

[R75] 导出环境变量
来源：http://nfd.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://dei.0kj1m.cn

[R76] 使用临时文件
来源：http://uln.xylfe.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vmn.mhx1999.top

[R77] 读取用户输入
来源：http://ccs.dianchejie.cn

read -rp "请输入: " ans
来源：http://zsp.svipenyu.cn

[R78] 交互式菜单
来源：http://usn.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vjo.jyoumei.cn

[R79] 解析命令行选项
来源：http://psu.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fmk.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://zzt.316326.xyz

time ./run.sh
来源：http://xie.gotoacloud.top

================================================================================
来源：http://wqb.shanyushiyangtech.top

S. C / C++ 专题
来源：http://gzf.tianlin.xyz

================================================================================
来源：http://aln.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://zhh.haohaochexian.top

#include <stdio.h>
来源：http://yby.guannengcc.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fkk.fengsongda.top

[S02] C：变量与格式化输出
来源：http://gkk.9152youxi.cn

int a = 10; printf("%d\n", a);
来源：http://yxn.bbcook.cn

[S03] C：读入整数
来源：http://hyw.yongpay.top

int x; scanf("%d", &x);
来源：http://oah.ivvv.top

[S04] C：字符串复制
来源：http://xqb.jiagoushi.top

char dst[32]; strcpy(dst, "hi");
来源：http://jox.iojbl.cn

[S05] C：字符串长度
来源：http://loq.snrcjt.cn

strlen(s)
来源：http://pcd.iojbl.cn

[S06] C：字符串比较
来源：http://lcu.snrcjt.cn

strcmp(a, b) == 0
来源：http://jsi.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://wgs.sysykeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ggy.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://ulf.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zfg.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://gyb.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mxm.ppjwa.cn

[S10] C：指针与解引用
来源：http://ohc.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://asc.meibo888.top

[S11] C：逐行读文件
来源：http://wkt.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://zww.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hnf.wangdashe.top

fclose(f);
来源：http://qvy.svipenyu.cn

[S12] C：写文件
来源：http://qxr.fanxiaobao.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jmr.sufxvd.cn

[S13] C：宏定义
来源：http://bsp.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bag.yj202588.top

[S14] C：枚举
来源：http://pfb.sxryk.cn

enum Color { RED, GREEN, BLUE };
来源：http://mqb.jyoumei.cn

[S15] C：类型转换
来源：http://ooa.sxryk.cn

(double) a / b
来源：http://dcm.zhoulong.xyz

[S16] C：位操作置位
来源：http://kcf.daria6918.cn

x |= (1 << 3);
来源：http://tuv.bbcook.cn

[S17] C：安全拼接字符串
来源：http://lbr.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fcf.pycfn.com

[S18] C：命令行参数
来源：http://zjp.haohaochexian.top

int main(int argc, char **argv)
来源：http://fdl.redwolf501.top

[S19] C：快速排序
来源：http://aas.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bwt.zhoulong.xyz

[S20] C：二分查找
来源：http://yne.ivvv.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hrk.jqgufenzy.top

[S21] C：字符类别判断
来源：http://qgv.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kxl.shangyingyoupin.top

[S22] C：字符串转数字
来源：http://srd.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ack.yueranfly.top

[S23] C：随机数
来源：http://xnu.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://psh.fehbvm.com

[S24] C：获取本地时间
来源：http://xdl.cdnleiting.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://obo.hnxiangtu.top

[S25] C：内存拷贝
来源：http://iyb.sweek.top

memcpy(dst, src, n);
来源：http://imo.nanxuanxn.top

[S26] C：内存清零
来源：http://tua.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://rmi.hywenlv.cn

[S27] C：定义常量
来源：http://wxd.hnxiangtu.top

const double PI = 3.14159;
来源：http://fwd.hysaishi.cn

[S28] C：静态变量
来源：http://fvb.xingfuxueyuan.xyz

static int counter = 0;
来源：http://rgr.bbcook.cn

[S29] C：变参函数
来源：http://xhd.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://thr.jlsjyb.cn

[S30] C：头文件保护
来源：http://pcz.hnxiangtu.top

#ifndef X_H
来源：http://qzx.tarul.cn

#define X_H
来源：http://izr.hnqzz.top

#endif
来源：http://jvn.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://ihy.tianlin.xyz

#include <iostream>
来源：http://xjx.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://irl.tarul.cn

[S32] C++：字符串
来源：http://nne.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://rdk.quarkkingdee.top

[S33] C++：vector 增删
来源：http://omq.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://doi.nanxinkj.top

[S34] C++：遍历 vector
来源：http://fqp.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://etn.hywenlv.cn

[S35] C++：map
来源：http://stf.hesvh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hfj.yonumen.top

[S36] C++：unordered_map
来源：http://arl.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jii.ydzc1.top

[S37] C++：set
来源：http://hrd.uphjek.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rfe.xziqi.cn

[S38] C++：排序
来源：http://ddj.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://wag.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://zgm.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://set.birdmap.top

[S40] C++：查找元素
来源：http://vfs.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qaf.hammf.cn


<!-- 参考信息 -->