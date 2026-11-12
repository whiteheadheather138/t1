代发 wailian999

[Q80] 字符串截取
来源：http://fgj.cdnleiting.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qzq.xziqi.cn

[Q81] 字符串替换
来源：http://qje.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wna.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://rfy.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wzy.bjfxy.top

[Q83] 大小写转换
来源：http://mgx.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://don.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://ynv.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://mpl.zhixingplan.top

[Q85] 数值取整
来源：http://kgh.jiagoushi.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qib.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://wip.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://guo.birdmap.top

[Q87] JSON 字段做条件
来源：http://pnq.shanyushiyangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kft.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://wdj.zdqjudy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hgd.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oea.fehbvm.com

[Q89] 判断表是否存在
来源：http://fgg.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hqm.cqqwz.cn

[Q90] 生成序号列
来源：http://yad.guowangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jnf.ehwqpu.com

================================================================================
来源：http://xtp.uphjek.com

R. Bash 专题
来源：http://aeq.yangfankeji.com

================================================================================
来源：http://ouk.cqqwz.cn

[R01] shebang 与严格模式
来源：http://iyc.kuanghao11.cn

#!/usr/bin/env bash
来源：http://ufq.316326.xyz

set -euo pipefail
来源：http://fyt.jiagoushi.top

[R02] 变量赋值与使用
来源：http://box.cashguo.top

name="Tom"; echo "$name"
来源：http://udt.316326.xyz

[R03] 只读变量
来源：http://jra.yj202588.top

readonly PI=3.14
来源：http://wkv.zhixingplan.top

[R04] 位置参数
来源：http://lio.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wkn.ivvv.top

[R05] 参数默认值
来源：http://xir.jqgufenzy.top

name="${1:-default}"
来源：http://vyj.yongpay.top

[R06] 判断命令是否存在
来源：http://klk.sufxvd.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zwz.9152youxi.cn

[R07] if 判断文件
来源：http://baq.xinyue.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ahc.birdmap.top

[R08] 数值比较
来源：http://lwm.haohaochexian.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uxs.iojbl.cn

[R09] 字符串比较
来源：http://cid.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nrx.mhx1999.top

[R10] 正则匹配
来源：http://fnz.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://atr.tianlin.xyz

[R11] case 多分支
来源：http://mhx.hysaishi.cn

case "$1" in
来源：http://sba.fehbvm.com

start) echo "启动" ;;
来源：http://rcl.snrcjt.cn

stop)  echo "停止" ;;
来源：http://sun.ybcxt.top

*)     echo "未知命令" ;;
来源：http://ieq.xinyue.icu

esac
来源：http://fyt.aibaodan.cn

[R12] for 遍历文件
来源：http://mfi.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://tjr.aizwys.cn

[R13] for 计数循环
来源：http://lpt.birdmap.top

for i in {1..10}; do echo "$i"; done
来源：http://wmt.zdqjudy.top

[R14] C 风格 for
来源：http://gmo.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fxt.pycfn.com

[R15] while 逐行读文件
来源：http://unh.fanxiaobao.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://apl.yanxiufei.cn

[R16] until 等待条件
来源：http://gao.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mvn.ybcxt.top

[R17] 数组定义与取值
来源：http://nmu.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://uji.zhixingplan.top

[R18] 遍历数组
来源：http://iaz.pengpengdd.cyou

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ado.yj20258888.top

[R19] 数组长度
来源：http://wts.ctjpmb.com

echo "${#arr[@]}"
来源：http://gxm.snrcjt.cn

[R20] 关联数组（字典）
来源：http://rme.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yge.feifeiyinyue.top

[R21] 字符串长度
来源：http://kfz.dianchejie.cn

echo "${#s}"
来源：http://rsv.sxryk.cn

[R22] 截取子串
来源：http://kta.yanxiufei.cn

echo "${s:0:5}"
来源：http://zhg.yangfankeji.com

[R23] 字符串替换
来源：http://nre.guowangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://acn.316326.xyz

[R24] 大小写转换
来源：http://zvk.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://wug.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://xtb.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kff.smart0.xyz

[R26] 命令替换
来源：http://kkk.sxryk.cn

now=$(date +%F); echo "$now"
来源：http://dtc.jinyuanbaomall.cn

[R27] 算术展开
来源：http://wht.hammf.cn

echo $((1 + 2 * 3))
来源：http://uld.zhongyouzk.top

[R28] 浮点运算
来源：http://uag.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://zyq.9152youxi.cn

[R29] 定义函数
来源：http://qrz.jlsjyb.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rry.cdnleiting.top

[R30] 函数返回状态码
来源：http://vlh.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://kvw.haohaochexian.top

[R31] 局部变量
来源：http://ntz.0kj1m.cn

f() { local x=1; echo "$x"; }
来源：http://cwm.ybcxt.top

[R32] 参数个数校验
来源：http://hee.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ifh.yueranfly.top

[R33] 捕获错误并提示行号
来源：http://xpg.zhongyouzk.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://siv.hysaishi.cn

[R34] 退出时清理
来源：http://vfl.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pgw.iojbl.cn

[R35] 后台执行并等待
来源：http://wzq.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cvt.jiagoushi.top

[R36] 并发执行多个任务
来源：http://owx.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tsv.shuidangran.top

[R37] 把输出赋给变量
来源：http://jeo.daxiang520.top

files=$(ls -1)
来源：http://qhl.jianghu66.top

[R38] 管道串联
来源：http://zgc.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://isy.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://pqj.meibo888.top

cmd > out.log 2>&1
来源：http://eiq.316326.xyz

[R40] 追加写日志
来源：http://qax.xuanzx.com

echo "log" >> out.log
来源：http://rox.pycfn.com

[R41] 丢弃输出
来源：http://vtr.iojbl.cn

cmd >/dev/null 2>&1
来源：http://psf.chenlongwang.top

[R42] 输入重定向
来源：http://yrd.xinyue.icu

wc -l < a.txt
来源：http://kxr.quarkkingdee.top

[R43] 按名字查找文件
来源：http://pbc.fzhhl.top

find . -name "*.log" -type f
来源：http://fyl.9152youxi.cn

[R44] 按修改时间查找
来源：http://oyx.zhongyouzk.top

find . -mtime -7 -type f
来源：http://acc.ywan-chungtsiang.top

[R45] 批量删除
来源：http://mhu.tanke756.top

find . -name "*.tmp" -delete
来源：http://kpd.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://sza.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iyl.chenjidiqi.icu

[R47] sed 单行替换
来源：http://xlw.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://shj.hysaishi.cn

[R48] awk 取指定列
来源：http://zcu.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://alx.hammf.cn

[R49] awk 带条件
来源：http://nix.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hgk.xuetiantiany.cn

[R50] awk 求和
来源：http://vei.guannengcc.top

awk '{s += $2} END {print s}' a.txt
来源：http://jce.tanke756.top

[R51] 排序去重取前几
来源：http://mlm.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lcb.jinghuilouyu.cn

[R52] 统计行数
来源：http://btp.xuetiantiany.cn

wc -l a.txt
来源：http://cxn.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://vlv.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kvj.fehbvm.com

[R54] 比较两个文件
来源：http://iml.yangfankeji.com

diff a.txt b.txt
来源：http://myv.ppjwa.cn

[R55] 压缩与解压
来源：http://pyz.epnwcf.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ohe.gotoacloud.top

[R56] 远程拷贝
来源：http://xko.redwolf501.top

scp file user@host:/path/
来源：http://dmb.hywenlv.cn

[R57] 远程执行命令
来源：http://gai.vehdjk.com

ssh user@host 'uptime'
来源：http://kbp.gotoacloud.top

[R58] 下载文件
来源：http://dkt.wangshuangyany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ytw.yj20258888.top

[R59] 发 POST JSON
来源：http://nap.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mbo.gaohongyu789.top

[R60] 只看 HTTP 状态码
来源：http://tya.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dci.sysykeji.top

[R61] 磁盘占用
来源：http://ryc.mhx1999.top

df -h;  du -sh *
来源：http://pcd.wangdashe.top

[R62] 找最占空间的文件
来源：http://yaw.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://gjh.svipenyu.cn

[R63] 内存与进程
来源：http://toc.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://hep.daria6918.cn

[R64] 结束进程
来源：http://dta.hesvh.cn

kill -9 $(pgrep -f app.py)
来源：http://grj.yj202588.top

[R65] 查看端口占用
来源：http://xec.ydzc1.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yxx.havefunace.top

[R66] 定时任务
来源：http://cii.316326.xyz

crontab -e;  crontab -l
来源：http://ijl.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://goz.sysykeji.top

openssl rand -hex 16
来源：http://hfk.ivvv.top

[R68] 计算文件校验值
来源：http://owz.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://ywj.quarkkingdee.top

[R69] 生成随机密码
来源：http://swb.aizwys.cn

head -c 16 /dev/urandom | base64
来源：http://kde.ivvv.top

[R70] 时间戳与互转
来源：http://iam.ivvv.top

date +%s;  date -d @1700000000
来源：http://ytp.guannengcc.top

[R71] 日期格式化
来源：http://jka.chenjidiqi.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://jvg.jiagoushi.top

[R72] 等待端口就绪
来源：http://oyb.nwbrower.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xee.hongshengwenyu.top

[R73] 分割大日志
来源：http://jty.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://vrd.vehdjk.com

[R74] 批量重命名
来源：http://hec.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lzz.ehwqpu.com

[R75] 导出环境变量
来源：http://hqt.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://xip.vqdsnc.cn

[R76] 使用临时文件
来源：http://uwc.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fmk.nanxinkj.top

[R77] 读取用户输入
来源：http://qjz.pycfn.com

read -rp "请输入: " ans
来源：http://yme.cashguo.top

[R78] 交互式菜单
来源：http://vfj.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lud.hysaishi.cn

[R79] 解析命令行选项
来源：http://gtk.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vpc.hammf.cn

[R80] 查看脚本执行耗时
来源：http://byd.jinqigfzy.top

time ./run.sh
来源：http://zlw.svipenyu.cn

================================================================================
来源：http://wvr.ivvv.top

S. C / C++ 专题
来源：http://bsf.zycfv.cn

================================================================================
来源：http://opf.gaohongyu789.top

[S01] C：Hello World
来源：http://pme.epnwcf.com

#include <stdio.h>
来源：http://vdo.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fhv.hesvh.cn

[S02] C：变量与格式化输出
来源：http://uvd.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://yrg.hcnkem.com

[S03] C：读入整数
来源：http://ffy.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://jwa.c1oappe.top

[S04] C：字符串复制
来源：http://irt.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gdp.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://jxm.hfpthk.cn

strlen(s)
来源：http://dms.ydjk.org.cn

[S06] C：字符串比较
来源：http://ljs.yanxiufei.cn

strcmp(a, b) == 0
来源：http://sbm.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://njv.0kj1m.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uub.guowangkeji.top

[S08] C：动态内存分配与释放
来源：http://rjg.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tjc.birdmap.top

[S09] C：结构体定义与初始化
来源：http://jfy.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lfs.hnqzz.top

[S10] C：指针与解引用
来源：http://obj.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://ybf.tanke756.top

[S11] C：逐行读文件
来源：http://qny.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://ntq.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kgz.shanyushiyangkeji.top

fclose(f);
来源：http://ryh.aizwys.cn

[S12] C：写文件
来源：http://xck.zhixingplan.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qha.gogol.net.cn

[S13] C：宏定义
来源：http://yfh.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jha.316326.xyz

[S14] C：枚举
来源：http://lwt.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://ttk.nwbrower.top

[S15] C：类型转换
来源：http://hgk.jqgfzy.top

(double) a / b
来源：http://ozc.smart0.xyz

[S16] C：位操作置位
来源：http://ray.yj20258.top

x |= (1 << 3);
来源：http://gfb.c1oappe.top

[S17] C：安全拼接字符串
来源：http://lqe.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wbc.vehdjk.com

[S18] C：命令行参数
来源：http://hhq.zycfv.cn

int main(int argc, char **argv)
来源：http://htl.chenzaomai.com

[S19] C：快速排序
来源：http://rqr.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mpi.sjlbkw.cn

[S20] C：二分查找
来源：http://frx.ydzc1.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://boo.sxryk.cn

[S21] C：字符类别判断
来源：http://rhb.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ash.yj20258888.top

[S22] C：字符串转数字
来源：http://ije.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://yxi.wangshuangyany.cn

[S23] C：随机数
来源：http://znz.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qdh.cdnleiting.top

[S24] C：获取本地时间
来源：http://ter.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zka.ehwqpu.com

[S25] C：内存拷贝
来源：http://vgk.zhengqikj.top

memcpy(dst, src, n);
来源：http://sms.zhengqikj.top

[S26] C：内存清零
来源：http://iyk.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://pla.epnwcf.com

[S27] C：定义常量
来源：http://xtp.cdnleiting.top

const double PI = 3.14159;
来源：http://uxi.xziqi.cn

[S28] C：静态变量
来源：http://oem.316326.xyz

static int counter = 0;
来源：http://cwl.yuanzhike.top

[S29] C：变参函数
来源：http://rhg.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xdu.chenjidiqi.icu

[S30] C：头文件保护
来源：http://zkv.aizwys.cn

#ifndef X_H
来源：http://qbu.pycfn.com

#define X_H
来源：http://aqx.dianchejie.cn

#endif
来源：http://srg.hywenlv.cn

[S31] C++：Hello World
来源：http://pzl.xziqi.cn

#include <iostream>
来源：http://gys.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://xmx.pengpengdd.cyou

[S32] C++：字符串
来源：http://lfo.hesvh.cn

std::string s = "hi";  s += "!";
来源：http://twd.fanxiaobao.xyz

[S33] C++：vector 增删
来源：http://ugb.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ysk.zhixingplan.top

[S34] C++：遍历 vector
来源：http://bvk.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://pio.jyoumei.cn

[S35] C++：map
来源：http://mve.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zdy.zdbjq.cn

[S36] C++：unordered_map
来源：http://guv.daria6918.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://smq.yfazqb.com

[S37] C++：set
来源：http://wyk.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://stk.vehdjk.com

[S38] C++：排序
来源：http://veh.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://nsj.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://bgx.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aed.sjlbkw.cn

[S40] C++：查找元素
来源：http://uua.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dnb.dashuyun.cn

[S41] C++：类与构造函数
来源：http://uus.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qdf.fktsv.cn

[S42] C++：继承与虚函数
来源：http://bix.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://xxf.sysykeji.top

[S43] C++：智能指针
来源：http://mgb.hammf.cn

auto p = std::make_unique<int>(5);
来源：http://wie.guowangkeji.top

[S44] C++：引用传参
来源：http://bxy.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://lma.shzxlz.cn

[S45] C++：lambda
来源：http://vwa.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://lzl.fehbvm.com

[S46] C++：函数模板
来源：http://yoi.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vjx.cucudq.cn

[S47] C++：结构化绑定遍历
来源：http://oak.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wwi.tianlin.xyz

[S48] C++：逐行读文件
来源：http://qtt.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vlv.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://nvt.meibo888.top

[S49] C++：写文件
来源：http://aiu.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zjg.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://lxo.shuidangran.top


<!-- 参考信息 -->