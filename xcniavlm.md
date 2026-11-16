代发 wailian999

SHOW INDEX FROM users;
来源：http://vph.pengpengdd.cyou

[Q73] 查看表状态
来源：http://cfs.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://utd.daria6918.cn

[Q74] 强制使用索引
来源：http://dwk.zycfv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hge.bbcook.cn

[Q75] 日期格式化
来源：http://fog.tarul.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qzm.xingfuxueyuan.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ocw.yuanzhike.top

[Q76] 按天统计
来源：http://jlk.zhoulong.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mcz.sjlbkw.cn

[Q77] 时间加减
来源：http://tyv.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dtj.dianchejie.cn

[Q78] 当前时间
来源：http://ppv.jinqigfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xiu.ybcxt.top

[Q79] 字符串拼接
来源：http://vmn.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yik.dashuyun.cn

[Q80] 字符串截取
来源：http://gsy.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lck.jinqigfzy.top

[Q81] 字符串替换
来源：http://mwt.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hzs.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://uoc.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sdh.kuanghao11.cn

[Q83] 大小写转换
来源：http://ogg.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fem.sxryk.cn

[Q84] 去除首尾空格
来源：http://mtp.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://rva.haohaochexian.top

[Q85] 数值取整
来源：http://mov.sjlbkw.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ziu.tanke756.top

[Q86] 读取 JSON 字段
来源：http://ogi.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rvj.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://xno.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iqt.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://weg.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lge.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zno.yfazqb.com

[Q89] 判断表是否存在
来源：http://mqg.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://axg.snrcjt.cn

[Q90] 生成序号列
来源：http://wog.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jii.zdbjq.cn

================================================================================
来源：http://pfb.cdnleiting.top

R. Bash 专题
来源：http://ljj.nwbrower.top

================================================================================
来源：http://qce.yongpay.top

[R01] shebang 与严格模式
来源：http://qpy.hywenlv.cn

#!/usr/bin/env bash
来源：http://zmu.yj202588.top

set -euo pipefail
来源：http://ngg.feifeiyinyue.top

[R02] 变量赋值与使用
来源：http://oam.fzhhl.top

name="Tom"; echo "$name"
来源：http://faz.316326.xyz

[R03] 只读变量
来源：http://lpe.zhengqikj.top

readonly PI=3.14
来源：http://zvk.xinyue.icu

[R04] 位置参数
来源：http://eik.yuxming.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vne.cdnleiting.top

[R05] 参数默认值
来源：http://eke.yj20258888.top

name="${1:-default}"
来源：http://skr.hnqzz.top

[R06] 判断命令是否存在
来源：http://zve.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iwh.jqgfzy.top

[R07] if 判断文件
来源：http://ife.ywan-chungtsiang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bxc.shuidangran.top

[R08] 数值比较
来源：http://opt.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ocz.tian-w.cn

[R09] 字符串比较
来源：http://cry.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wcl.xylfe.cn

[R10] 正则匹配
来源：http://stz.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://enm.xuanzx.com

[R11] case 多分支
来源：http://jxi.birdmap.top

case "$1" in
来源：http://sos.yj20258.top

start) echo "启动" ;;
来源：http://orq.meibo888.top

stop)  echo "停止" ;;
来源：http://bba.jinqigufen.top

*)     echo "未知命令" ;;
来源：http://eyu.feifeiyinyue.top

esac
来源：http://mnl.sxryk.cn

[R12] for 遍历文件
来源：http://whk.ybcxt.top

for f in *.txt; do echo "$f"; done
来源：http://jww.zhoulong.xyz

[R13] for 计数循环
来源：http://ugq.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://hei.ehwqpu.com

[R14] C 风格 for
来源：http://mlw.dashuyun.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://man.kuanghao11.cn

[R15] while 逐行读文件
来源：http://tpn.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gcs.jlsjyb.cn

[R16] until 等待条件
来源：http://qvv.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bmd.hnxiangtu.top

[R17] 数组定义与取值
来源：http://cex.mhx1999.top

arr=(a b c); echo "${arr[0]}"
来源：http://qcu.xziqi.cn

[R18] 遍历数组
来源：http://rze.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://egv.jiagoushi.top

[R19] 数组长度
来源：http://zgj.yangfankeji.com

echo "${#arr[@]}"
来源：http://pdh.ybcxt.top

[R20] 关联数组（字典）
来源：http://zzi.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uqe.chenjidiqi.icu

[R21] 字符串长度
来源：http://zkb.ydjk.org.cn

echo "${#s}"
来源：http://hiy.birdmap.top

[R22] 截取子串
来源：http://fos.tianlin.xyz

echo "${s:0:5}"
来源：http://tdh.meibo888.top

[R23] 字符串替换
来源：http://qbs.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ycb.vqdsnc.cn

[R24] 大小写转换
来源：http://ced.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gzl.guannengcc.top

[R25] 去后缀 / 去前缀
来源：http://bnx.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zpw.xuetiantiany.cn

[R26] 命令替换
来源：http://upr.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://gms.316326.xyz

[R27] 算术展开
来源：http://yiy.xuanzx.com

echo $((1 + 2 * 3))
来源：http://cki.feifeiyinyue.top

[R28] 浮点运算
来源：http://ksu.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://ndu.havefunace.top

[R29] 定义函数
来源：http://fzx.zhijiandao.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wqc.dianchejie.cn

[R30] 函数返回状态码
来源：http://dju.smart0.xyz

f() { return 0; }; f || echo "失败了"
来源：http://dbj.uphjek.com

[R31] 局部变量
来源：http://fnk.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://gve.fktsv.cn

[R32] 参数个数校验
来源：http://bfv.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tcb.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://kwj.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hxy.tian-w.cn

[R34] 退出时清理
来源：http://lzg.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ehl.yj202588.top

[R35] 后台执行并等待
来源：http://jjc.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wco.wangshuangyany.cn

[R36] 并发执行多个任务
来源：http://htt.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pqm.hywenlv.cn

[R37] 把输出赋给变量
来源：http://vaz.52xcode.cn

files=$(ls -1)
来源：http://bgw.nanxinkj.top

[R38] 管道串联
来源：http://ejn.xziqi.cn

cat a.txt | grep -i error | wc -l
来源：http://quq.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://wsl.cdnleiting.top

cmd > out.log 2>&1
来源：http://fag.pengpengdd.cyou

[R40] 追加写日志
来源：http://ptp.aibaodan.cn

echo "log" >> out.log
来源：http://wvm.chenzaomai.com

[R41] 丢弃输出
来源：http://iut.uphjek.com

cmd >/dev/null 2>&1
来源：http://cbp.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://wjp.yvedp.cn

wc -l < a.txt
来源：http://cum.sysykeji.top

[R43] 按名字查找文件
来源：http://sak.fzhhl.top

find . -name "*.log" -type f
来源：http://rys.meibo888.top

[R44] 按修改时间查找
来源：http://iwn.dianchejie.cn

find . -mtime -7 -type f
来源：http://lip.xuetiantiany.cn

[R45] 批量删除
来源：http://fpw.zhongyouzk.top

find . -name "*.tmp" -delete
来源：http://wub.aibaodan.cn

[R46] 递归替换文件内容
来源：http://jdw.hfpthk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mig.bbcook.cn

[R47] sed 单行替换
来源：http://bju.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nfi.hcnkem.com

[R48] awk 取指定列
来源：http://vwn.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://sly.haohaochexian.top

[R49] awk 带条件
来源：http://cls.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eza.svipenyu.cn

[R50] awk 求和
来源：http://bot.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tuy.sweek.top

[R51] 排序去重取前几
来源：http://vcn.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ukk.ydzc1.top

[R52] 统计行数
来源：http://vqt.jlsjyb.cn

wc -l a.txt
来源：http://apw.cheryme.top

[R53] 查看文件头与实时尾
来源：http://hnw.tianlin.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lme.cdnleiting.top

[R54] 比较两个文件
来源：http://aka.dashuyun.cn

diff a.txt b.txt
来源：http://nah.ehwqpu.com

[R55] 压缩与解压
来源：http://gzc.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dvz.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://trj.kuanghao11.cn

scp file user@host:/path/
来源：http://ixv.zhiwuduotai.top

[R57] 远程执行命令
来源：http://uxu.xuanzx.com

ssh user@host 'uptime'
来源：http://mwa.jinqigfzy.top

[R58] 下载文件
来源：http://mvh.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rhr.yj20258.top

[R59] 发 POST JSON
来源：http://bsr.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hsn.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://hxz.wangshuangyany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zji.fengsongda.top

[R61] 磁盘占用
来源：http://pmb.jinqigufen.top

df -h;  du -sh *
来源：http://htk.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://xca.aizwys.cn

du -ah . | sort -rh | head -10
来源：http://bex.yuxming.cn

[R63] 内存与进程
来源：http://iwb.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://eox.9152youxi.cn

[R64] 结束进程
来源：http://pte.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://hyj.andypj.xyz

[R65] 查看端口占用
来源：http://fal.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ezw.cashguo.top

[R66] 定时任务
来源：http://kho.xingfuxueyuan.xyz

crontab -e;  crontab -l
来源：http://ikv.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://qip.yj20258.top

openssl rand -hex 16
来源：http://jch.bjfxy.top

[R68] 计算文件校验值
来源：http://euw.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tyz.vehdjk.com

[R69] 生成随机密码
来源：http://tkt.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://tdd.sjlbkw.cn

[R70] 时间戳与互转
来源：http://sqh.bbcook.cn

date +%s;  date -d @1700000000
来源：http://ovq.zycfv.cn

[R71] 日期格式化
来源：http://epm.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pye.zhijiandao.cn

[R72] 等待端口就绪
来源：http://bpq.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://yrr.tian-w.cn

[R73] 分割大日志
来源：http://prb.52xcode.cn

split -l 1000 big.log part_
来源：http://xrn.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://uwm.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dzg.jqgfzy.top

[R75] 导出环境变量
来源：http://kmn.hywenlv.cn

export PATH="$HOME/bin:$PATH"
来源：http://eqc.52xcode.cn

[R76] 使用临时文件
来源：http://isq.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nkl.tian-w.cn

[R77] 读取用户输入
来源：http://dbb.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://wtq.quarkkingdee.top

[R78] 交互式菜单
来源：http://vkr.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yah.sjlbkw.cn

[R79] 解析命令行选项
来源：http://myc.hongshengwenyu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ecj.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://mie.smart0.xyz

time ./run.sh
来源：http://iqr.nwbrower.top

================================================================================
来源：http://qms.vqdsnc.cn

S. C / C++ 专题
来源：http://dbr.xziqi.cn

================================================================================
来源：http://uwu.c1oappe.top

[S01] C：Hello World
来源：http://iuv.feifeiyinyue.top

#include <stdio.h>
来源：http://rqk.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uij.daxiang520.top

[S02] C：变量与格式化输出
来源：http://avz.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://rvk.gaohongyu789.top

[S03] C：读入整数
来源：http://sps.chenzaomai.com

int x; scanf("%d", &x);
来源：http://oxt.yonumen.top

[S04] C：字符串复制
来源：http://jei.zdbjq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://now.jyoumei.cn

[S05] C：字符串长度
来源：http://quf.yfazqb.com

strlen(s)
来源：http://okv.fzhhl.top

[S06] C：字符串比较
来源：http://gyh.sufxvd.cn

strcmp(a, b) == 0
来源：http://dxs.zdqjudy.top

[S07] C：数组遍历求和
来源：http://dmi.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nru.yj20258.top

[S08] C：动态内存分配与释放
来源：http://okj.sysykeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oke.smart0.xyz

[S09] C：结构体定义与初始化
来源：http://ofy.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zva.shzxlz.cn

[S10] C：指针与解引用
来源：http://hbw.ybcxt.top

int *p = &a;  *p = 5;
来源：http://twu.smart0.xyz

[S11] C：逐行读文件
来源：http://ggw.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://fkt.jinyuanbaomall.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tre.shanyushiyangtech.top

fclose(f);
来源：http://neu.pengpengdd.cyou

[S12] C：写文件
来源：http://ntf.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rsy.0kj1m.cn

[S13] C：宏定义
来源：http://abz.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mre.jinqigfzy.top

[S14] C：枚举
来源：http://ndg.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://sew.nanxuanxn.top

[S15] C：类型转换
来源：http://aaw.wangdashe.top

(double) a / b
来源：http://tcb.hfpthk.cn

[S16] C：位操作置位
来源：http://zzq.gogol.net.cn

x |= (1 << 3);
来源：http://zjz.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://pjp.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gsy.yueranfly.top

[S18] C：命令行参数
来源：http://tgh.52xcode.cn

int main(int argc, char **argv)
来源：http://yyj.tarul.cn

[S19] C：快速排序
来源：http://mli.cqqwz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ouy.hysaishi.cn

[S20] C：二分查找
来源：http://aib.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sta.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://spa.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://agp.quarkkingdee.top

[S22] C：字符串转数字
来源：http://ssz.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://elj.tianlin.xyz

[S23] C：随机数
来源：http://dcw.guannengcc.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pew.cucudq.cn

[S24] C：获取本地时间
来源：http://iib.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hqy.snrcjt.cn

[S25] C：内存拷贝
来源：http://ppi.nanxinkj.top

memcpy(dst, src, n);
来源：http://otf.yfazqb.com

[S26] C：内存清零
来源：http://eqn.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://vvl.hnxiangtu.top

[S27] C：定义常量
来源：http://pga.iojbl.cn

const double PI = 3.14159;
来源：http://jgs.aizwys.cn

[S28] C：静态变量
来源：http://qti.chenlongwang.top

static int counter = 0;
来源：http://qbn.gotoacloud.top

[S29] C：变参函数
来源：http://kuj.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pgk.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://nww.hysaishi.cn

#ifndef X_H
来源：http://ajz.fanxiaobao.xyz

#define X_H
来源：http://ebp.sxryk.cn

#endif
来源：http://uyp.chenlongwang.top

[S31] C++：Hello World
来源：http://qpv.meibo888.top

#include <iostream>
来源：http://scj.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://zpu.zhengqikj.top

[S32] C++：字符串
来源：http://ibl.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://fmj.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://naq.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wgz.ybcxt.top

[S34] C++：遍历 vector
来源：http://eao.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://qdb.bjfxy.top

[S35] C++：map
来源：http://oab.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ksu.cheryme.top

[S36] C++：unordered_map
来源：http://xjt.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fyr.hywenlv.cn

[S37] C++：set
来源：http://wop.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ohe.mhx1999.top

[S38] C++：排序
来源：http://mlw.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://wgw.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://fvk.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uzl.pengpengdd.cyou

[S40] C++：查找元素
来源：http://rda.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tua.uphjek.com

[S41] C++：类与构造函数
来源：http://zdp.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://asi.gaohongyu789.top

[S42] C++：继承与虚函数
来源：http://zpj.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://tey.xuetiantiany.cn


<!-- 参考信息 -->