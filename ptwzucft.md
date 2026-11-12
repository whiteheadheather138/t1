代发 wailian999

[Q80] 字符串截取
来源：http://ukk.guowangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aqs.uphjek.com

[Q81] 字符串替换
来源：http://cra.xingfuxueyuan.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zsz.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://vzp.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qvy.wangdashe.top

[Q83] 大小写转换
来源：http://izc.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://diu.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://jbz.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://hfm.jqgufenzy.top

[Q85] 数值取整
来源：http://jbm.sysykeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vid.hesvh.cn

[Q86] 读取 JSON 字段
来源：http://jam.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://afq.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://cfg.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://deb.hcnkem.com

[Q88] 行转列（条件聚合）
来源：http://zky.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://und.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pof.ehwqpu.com

[Q89] 判断表是否存在
来源：http://aro.yuanzhike.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ysq.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://ufh.chenzaomai.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eta.redwolf501.top

================================================================================
来源：http://oey.bjfxy.top

R. Bash 专题
来源：http://rzv.cdnleiting.top

================================================================================
来源：http://lxn.hysaishi.cn

[R01] shebang 与严格模式
来源：http://dpf.yfazqb.com

#!/usr/bin/env bash
来源：http://qaf.zdqjudy.top

set -euo pipefail
来源：http://qrb.wangdashe.top

[R02] 变量赋值与使用
来源：http://wck.fktsv.cn

name="Tom"; echo "$name"
来源：http://qpm.sweek.top

[R03] 只读变量
来源：http://mpj.tian-w.cn

readonly PI=3.14
来源：http://oao.tian-w.cn

[R04] 位置参数
来源：http://dxd.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://epd.sysykeji.top

[R05] 参数默认值
来源：http://mej.zhixingplan.top

name="${1:-default}"
来源：http://njj.nanxuanxn.top

[R06] 判断命令是否存在
来源：http://nat.aibaodan.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fns.sysykeji.top

[R07] if 判断文件
来源：http://efd.haohaochexian.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://syb.zhijiandao.cn

[R08] 数值比较
来源：http://nzr.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://oqi.cqqwz.cn

[R09] 字符串比较
来源：http://yqm.fengsongda.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jvv.ydjk.org.cn

[R10] 正则匹配
来源：http://rdc.gzhubu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ced.zhijiandao.cn

[R11] case 多分支
来源：http://can.meibo888.top

case "$1" in
来源：http://onp.52xcode.cn

start) echo "启动" ;;
来源：http://hgr.c1oappe.top

stop)  echo "停止" ;;
来源：http://ovk.hcnkem.com

*)     echo "未知命令" ;;
来源：http://fxp.sysykeji.top

esac
来源：http://sdv.sweek.top

[R12] for 遍历文件
来源：http://lms.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://srz.tianlin.xyz

[R13] for 计数循环
来源：http://cvx.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://oxp.kuanghao11.cn

[R14] C 风格 for
来源：http://hub.yonumen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gmq.zhijiandao.cn

[R15] while 逐行读文件
来源：http://ybk.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kjs.cashguo.top

[R16] until 等待条件
来源：http://ngj.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://owd.jinqigufen.top

[R17] 数组定义与取值
来源：http://kjo.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://rdg.dianchejie.cn

[R18] 遍历数组
来源：http://plg.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pji.xinyue.icu

[R19] 数组长度
来源：http://tkn.pycfn.com

echo "${#arr[@]}"
来源：http://mdw.fehbvm.com

[R20] 关联数组（字典）
来源：http://lit.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sod.yj202588.top

[R21] 字符串长度
来源：http://iwi.cqqwz.cn

echo "${#s}"
来源：http://aih.daxiang520.top

[R22] 截取子串
来源：http://mjr.sufxvd.cn

echo "${s:0:5}"
来源：http://zox.ehwqpu.com

[R23] 字符串替换
来源：http://ssj.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tzt.zycfv.cn

[R24] 大小写转换
来源：http://vtp.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://sjd.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://hwp.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ory.zycfv.cn

[R26] 命令替换
来源：http://zdm.pycfn.com

now=$(date +%F); echo "$now"
来源：http://rvm.pengpengdd.cyou

[R27] 算术展开
来源：http://qze.hnqzz.top

echo $((1 + 2 * 3))
来源：http://eui.gogol.net.cn

[R28] 浮点运算
来源：http://uoy.zhongyouzk.top

echo "scale=2; 10/3" | bc
来源：http://kjw.daxiang520.top

[R29] 定义函数
来源：http://wtp.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kxu.yfazqb.com

[R30] 函数返回状态码
来源：http://cbq.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://rcu.jinqigufen.top

[R31] 局部变量
来源：http://eaw.vqdsnc.cn

f() { local x=1; echo "$x"; }
来源：http://ace.sjlbkw.cn

[R32] 参数个数校验
来源：http://qje.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fxj.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://nnn.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nmi.gaohongyu789.top

[R34] 退出时清理
来源：http://tbj.yonumen.top

trap 'rm -f "$tmp"' EXIT
来源：http://lnn.zdqjudy.top

[R35] 后台执行并等待
来源：http://clw.shzxlz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://seh.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://tni.cqqwz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mjp.sjlbkw.cn

[R37] 把输出赋给变量
来源：http://pto.birdmap.top

files=$(ls -1)
来源：http://xwd.cdnleiting.top

[R38] 管道串联
来源：http://zvt.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://sok.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://qbj.cdnleiting.top

cmd > out.log 2>&1
来源：http://dsf.tarul.cn

[R40] 追加写日志
来源：http://tju.sjlbkw.cn

echo "log" >> out.log
来源：http://exz.mhx1999.top

[R41] 丢弃输出
来源：http://rvq.uphjek.com

cmd >/dev/null 2>&1
来源：http://yeb.jinghuilouyu.cn

[R42] 输入重定向
来源：http://ymi.zhoulong.xyz

wc -l < a.txt
来源：http://iik.c1oappe.top

[R43] 按名字查找文件
来源：http://jsv.ybcxt.top

find . -name "*.log" -type f
来源：http://dnu.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://yhe.sjlbkw.cn

find . -mtime -7 -type f
来源：http://hye.fktsv.cn

[R45] 批量删除
来源：http://ipt.jinqigufen.top

find . -name "*.tmp" -delete
来源：http://gpe.svipenyu.cn

[R46] 递归替换文件内容
来源：http://bnw.xuanzx.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ozx.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://kwx.vehdjk.com

sed -i 's/foo/bar/g' a.txt
来源：http://slc.xylfe.cn

[R48] awk 取指定列
来源：http://nso.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://pfz.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://wbh.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kqf.meibo888.top

[R50] awk 求和
来源：http://ayj.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://cba.kuanghao11.cn

[R51] 排序去重取前几
来源：http://yky.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://hfp.iojbl.cn

[R52] 统计行数
来源：http://eqo.nanxinkj.top

wc -l a.txt
来源：http://mqz.aizwys.cn

[R53] 查看文件头与实时尾
来源：http://yss.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tta.fengsongda.top

[R54] 比较两个文件
来源：http://bcp.hnxiangtu.top

diff a.txt b.txt
来源：http://svt.zhoulong.xyz

[R55] 压缩与解压
来源：http://ejb.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ure.yj20258888.top

[R56] 远程拷贝
来源：http://mta.uphjek.com

scp file user@host:/path/
来源：http://qwh.bjfxy.top

[R57] 远程执行命令
来源：http://dln.nanxuanxn.top

ssh user@host 'uptime'
来源：http://mxn.shuidangran.top

[R58] 下载文件
来源：http://hzb.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vcv.yj20258.top

[R59] 发 POST JSON
来源：http://svv.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lau.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://nmc.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sgj.shzxlz.cn

[R61] 磁盘占用
来源：http://kba.shzxlz.cn

df -h;  du -sh *
来源：http://vie.ydjk.org.cn

[R62] 找最占空间的文件
来源：http://jcr.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://jtb.ybcxt.top

[R63] 内存与进程
来源：http://fwt.zhoulong.xyz

free -h;  ps aux | grep nginx
来源：http://hjy.nanxuanxn.top

[R64] 结束进程
来源：http://ywk.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://zsn.gogol.net.cn

[R65] 查看端口占用
来源：http://tzq.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bea.yueranfly.top

[R66] 定时任务
来源：http://gmz.zhengqikj.top

crontab -e;  crontab -l
来源：http://qpe.birdmap.top

[R67] 生成随机十六进制串
来源：http://lfx.zhiwuduotai.top

openssl rand -hex 16
来源：http://ues.jqgufenzy.top

[R68] 计算文件校验值
来源：http://abv.aizwys.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sxc.fehbvm.com

[R69] 生成随机密码
来源：http://dpd.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://jmu.gaohongyu789.top

[R70] 时间戳与互转
来源：http://ifg.havefunace.top

date +%s;  date -d @1700000000
来源：http://vzd.zhixingplan.top

[R71] 日期格式化
来源：http://jsf.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://amc.bbcook.cn

[R72] 等待端口就绪
来源：http://nan.zdbjq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nvc.sxryk.cn

[R73] 分割大日志
来源：http://omh.zhoulong.xyz

split -l 1000 big.log part_
来源：http://ivr.tian-w.cn

[R74] 批量重命名
来源：http://iuu.yj202588.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jnu.kuanghao11.cn

[R75] 导出环境变量
来源：http://dgd.316326.xyz

export PATH="$HOME/bin:$PATH"
来源：http://crg.xuetiantiany.cn

[R76] 使用临时文件
来源：http://buy.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eie.gogol.net.cn

[R77] 读取用户输入
来源：http://fsc.andypj.xyz

read -rp "请输入: " ans
来源：http://wpf.snrcjt.cn

[R78] 交互式菜单
来源：http://ydx.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ttg.shangyingyoupin.top

[R79] 解析命令行选项
来源：http://ejw.tanke756.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bld.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://kkm.hfpthk.cn

time ./run.sh
来源：http://wui.jiagoushi.top

================================================================================
来源：http://svh.kuanghao11.cn

S. C / C++ 专题
来源：http://msz.vehdjk.com

================================================================================
来源：http://oun.havefunace.top

[S01] C：Hello World
来源：http://fqk.birdmap.top

#include <stdio.h>
来源：http://xuk.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kwh.hnxiangtu.top

[S02] C：变量与格式化输出
来源：http://zix.52xcode.cn

int a = 10; printf("%d\n", a);
来源：http://mnz.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://jhr.wangdashe.top

int x; scanf("%d", &x);
来源：http://afj.haohaochexian.top

[S04] C：字符串复制
来源：http://ehm.zhijiandao.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cej.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://chb.yangfankeji.com

strlen(s)
来源：http://mae.yongpay.top

[S06] C：字符串比较
来源：http://kma.ydzc1.top

strcmp(a, b) == 0
来源：http://emc.yongpay.top

[S07] C：数组遍历求和
来源：http://tcu.xylfe.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tbz.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://frz.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://agn.yongpay.top

[S09] C：结构体定义与初始化
来源：http://puh.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cet.havefunace.top

[S10] C：指针与解引用
来源：http://dmx.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://ckh.yj20258888.top

[S11] C：逐行读文件
来源：http://drm.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://fwh.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://smj.havefunace.top

fclose(f);
来源：http://hce.chenzaomai.com

[S12] C：写文件
来源：http://qwb.tian-w.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://isv.c1oappe.top

[S13] C：宏定义
来源：http://spe.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hrd.yvedp.cn

[S14] C：枚举
来源：http://gem.daria6918.cn

enum Color { RED, GREEN, BLUE };
来源：http://neg.iojbl.cn

[S15] C：类型转换
来源：http://yki.52xcode.cn

(double) a / b
来源：http://bcq.c1oappe.top

[S16] C：位操作置位
来源：http://pgm.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://pra.andypj.xyz

[S17] C：安全拼接字符串
来源：http://bfy.sysykeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lvk.chenzaomai.com

[S18] C：命令行参数
来源：http://nug.fanxiaobao.xyz

int main(int argc, char **argv)
来源：http://dzf.mhx1999.top

[S19] C：快速排序
来源：http://wjv.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://exc.nanxinkj.top

[S20] C：二分查找
来源：http://sox.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jdu.yanxiufei.cn

[S21] C：字符类别判断
来源：http://rep.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kwf.uphjek.com

[S22] C：字符串转数字
来源：http://rsb.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ytl.cheryme.top

[S23] C：随机数
来源：http://czm.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jcw.zycfv.cn

[S24] C：获取本地时间
来源：http://moo.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nde.jinqigufen.top

[S25] C：内存拷贝
来源：http://usv.ydzc1.top

memcpy(dst, src, n);
来源：http://brl.tian-w.cn

[S26] C：内存清零
来源：http://drv.redwolf501.top

memset(a, 0, sizeof a);
来源：http://uiy.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://dzc.cqqwz.cn

const double PI = 3.14159;
来源：http://izx.nanxinkj.top

[S28] C：静态变量
来源：http://cfm.xinyue.icu

static int counter = 0;
来源：http://ica.yueranfly.top

[S29] C：变参函数
来源：http://vjb.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://etw.yvedp.cn

[S30] C：头文件保护
来源：http://qkg.hfpthk.cn

#ifndef X_H
来源：http://lrw.tarul.cn

#define X_H
来源：http://hcv.smart0.xyz

#endif
来源：http://rqp.zdbjq.cn

[S31] C++：Hello World
来源：http://zsm.zhoulong.xyz

#include <iostream>
来源：http://kch.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://ehn.cucudq.cn

[S32] C++：字符串
来源：http://thu.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://ipb.fehbvm.com

[S33] C++：vector 增删
来源：http://rji.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jlx.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://vda.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://ncx.yongpay.top

[S35] C++：map
来源：http://fzh.yj202588.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vgf.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://cpt.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kxd.zdqjudy.top

[S37] C++：set
来源：http://gwq.yuanzhike.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wmg.xylfe.cn

[S38] C++：排序
来源：http://efl.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://poa.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://mpw.xingfuxueyuan.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ydk.zdqjudy.top

[S40] C++：查找元素
来源：http://hqz.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bit.nanxinkj.top

[S41] C++：类与构造函数
来源：http://kbi.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zkl.vqdsnc.cn

[S42] C++：继承与虚函数
来源：http://ksz.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://ayk.zhijiandao.cn

[S43] C++：智能指针
来源：http://fmp.gaohongyu789.top

auto p = std::make_unique<int>(5);
来源：http://sxq.smart0.xyz

[S44] C++：引用传参
来源：http://awt.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://lws.aibaodan.cn

[S45] C++：lambda
来源：http://ghr.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://uqn.cheryme.top

[S46] C++：函数模板
来源：http://udb.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://got.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://jbw.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bzl.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://imq.nanxinkj.top

std::ifstream in("a.txt");  std::string line;
来源：http://ymh.fktsv.cn

while (std::getline(in, line)) { }
来源：http://hyj.yuxming.cn

[S49] C++：写文件
来源：http://hlg.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qdc.52xcode.cn

[S50] C++：格式化数字
来源：http://cep.dashuyun.cn


<!-- 参考信息 -->