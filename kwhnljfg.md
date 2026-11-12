代发 wailian999

[Q86] 读取 JSON 字段
来源：http://jij.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rkt.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://uwu.cheryme.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ejn.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://fip.hesvh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://taw.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vuc.jyoumei.cn

[Q89] 判断表是否存在
来源：http://dyo.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dej.shuidangran.top

[Q90] 生成序号列
来源：http://dwe.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hyk.yuanzhike.top

================================================================================
来源：http://gai.wangshuangyany.cn

R. Bash 专题
来源：http://xws.ybcxt.top

================================================================================
来源：http://bvo.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://unx.guowangkeji.top

#!/usr/bin/env bash
来源：http://knt.aizwys.cn

set -euo pipefail
来源：http://kqk.zycfv.cn

[R02] 变量赋值与使用
来源：http://vos.ybcxt.top

name="Tom"; echo "$name"
来源：http://ccy.dianchejie.cn

[R03] 只读变量
来源：http://vnh.jqgufenzy.top

readonly PI=3.14
来源：http://knr.ybcxt.top

[R04] 位置参数
来源：http://fds.tianlin.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iux.hnqzz.top

[R05] 参数默认值
来源：http://wno.fengsongda.top

name="${1:-default}"
来源：http://lmn.xylfe.cn

[R06] 判断命令是否存在
来源：http://xni.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zjc.cheryme.top

[R07] if 判断文件
来源：http://kin.zhijiandao.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rzp.fzhhl.top

[R08] 数值比较
来源：http://omf.zhiwuduotai.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fvg.gzhubu.top

[R09] 字符串比较
来源：http://meq.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eqk.bbcook.cn

[R10] 正则匹配
来源：http://wrn.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://axo.bbcook.cn

[R11] case 多分支
来源：http://zgg.gzhubu.top

case "$1" in
来源：http://jth.guannengcc.top

start) echo "启动" ;;
来源：http://bmg.bjfxy.top

stop)  echo "停止" ;;
来源：http://chc.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://jkd.fanxiaobao.xyz

esac
来源：http://ehz.tian-w.cn

[R12] for 遍历文件
来源：http://qdb.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://ton.quarkkingdee.top

[R13] for 计数循环
来源：http://tsm.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://ghm.c1oappe.top

[R14] C 风格 for
来源：http://tos.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bvo.bjfxy.top

[R15] while 逐行读文件
来源：http://oaa.birdmap.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tee.zhoulong.xyz

[R16] until 等待条件
来源：http://pje.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mxj.kuanghao11.cn

[R17] 数组定义与取值
来源：http://stb.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://svq.cqqwz.cn

[R18] 遍历数组
来源：http://ihi.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yvk.yj20258.top

[R19] 数组长度
来源：http://tzp.hysaishi.cn

echo "${#arr[@]}"
来源：http://lgj.chenzaomai.com

[R20] 关联数组（字典）
来源：http://vsn.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yvb.ivvv.top

[R21] 字符串长度
来源：http://bgx.0kj1m.cn

echo "${#s}"
来源：http://llj.zhixingplan.top

[R22] 截取子串
来源：http://lsl.9152youxi.cn

echo "${s:0:5}"
来源：http://kkx.zhixingplan.top

[R23] 字符串替换
来源：http://chc.fktsv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://usc.wangshuangyany.cn

[R24] 大小写转换
来源：http://tak.yanxiufei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://plh.bbcook.cn

[R25] 去后缀 / 去前缀
来源：http://wmq.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jzt.havefunace.top

[R26] 命令替换
来源：http://lwh.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://nck.hnxiangtu.top

[R27] 算术展开
来源：http://eru.sweek.top

echo $((1 + 2 * 3))
来源：http://ddz.wangshuangyany.cn

[R28] 浮点运算
来源：http://ixv.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://jeo.fktsv.cn

[R29] 定义函数
来源：http://bxw.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rbf.yueranfly.top

[R30] 函数返回状态码
来源：http://wai.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://oep.vehdjk.com

[R31] 局部变量
来源：http://ckm.yj20258.top

f() { local x=1; echo "$x"; }
来源：http://eww.cqqwz.cn

[R32] 参数个数校验
来源：http://jtf.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gac.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://mxd.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gqo.zhongyouzk.top

[R34] 退出时清理
来源：http://ufh.chenjidiqi.icu

trap 'rm -f "$tmp"' EXIT
来源：http://mns.bbcook.cn

[R35] 后台执行并等待
来源：http://xks.zdqjudy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rqd.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://olg.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ptx.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://fsj.birdmap.top

files=$(ls -1)
来源：http://mym.cdnleiting.top

[R38] 管道串联
来源：http://zij.jqgfzy.top

cat a.txt | grep -i error | wc -l
来源：http://shk.chenlongwang.top

[R39] 重定向标准输出与错误
来源：http://rnl.pycfn.com

cmd > out.log 2>&1
来源：http://fyh.redwolf501.top

[R40] 追加写日志
来源：http://nuy.jianghu66.top

echo "log" >> out.log
来源：http://cfi.quarkkingdee.top

[R41] 丢弃输出
来源：http://uox.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://oxa.cashguo.top

[R42] 输入重定向
来源：http://otl.fanxiaobao.xyz

wc -l < a.txt
来源：http://gtu.hnqzz.top

[R43] 按名字查找文件
来源：http://moi.gaohongyu789.top

find . -name "*.log" -type f
来源：http://hzj.xylfe.cn

[R44] 按修改时间查找
来源：http://uff.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://edk.hfpthk.cn

[R45] 批量删除
来源：http://wyb.c1oappe.top

find . -name "*.tmp" -delete
来源：http://sqq.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://hpa.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gpw.hammf.cn

[R47] sed 单行替换
来源：http://tva.shanyushiyangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://wjo.dianchejie.cn

[R48] awk 取指定列
来源：http://jzs.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://ygl.gzhubu.top

[R49] awk 带条件
来源：http://xwe.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://moi.jinyuanbaomall.cn

[R50] awk 求和
来源：http://wwt.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mca.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://bcw.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pst.ppjwa.cn

[R52] 统计行数
来源：http://lod.sufxvd.cn

wc -l a.txt
来源：http://tud.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://pvn.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sha.ybcxt.top

[R54] 比较两个文件
来源：http://dzt.zhoulong.xyz

diff a.txt b.txt
来源：http://mwa.zdqjudy.top

[R55] 压缩与解压
来源：http://opq.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://klj.hnxiangtu.top

[R56] 远程拷贝
来源：http://obv.guannengcc.top

scp file user@host:/path/
来源：http://vvh.quarkkingdee.top

[R57] 远程执行命令
来源：http://apr.kuanghao11.cn

ssh user@host 'uptime'
来源：http://vlr.yuanzhike.top

[R58] 下载文件
来源：http://jrs.shuidangran.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ypd.tarul.cn

[R59] 发 POST JSON
来源：http://yju.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lpc.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://vde.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hmr.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://vkw.yonumen.top

df -h;  du -sh *
来源：http://ffe.daxiang520.top

[R62] 找最占空间的文件
来源：http://vqe.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://ybi.jiagoushi.top

[R63] 内存与进程
来源：http://ovz.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://huq.hongshengwenyu.top

[R64] 结束进程
来源：http://ulu.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://ltq.guannengcc.top

[R65] 查看端口占用
来源：http://mng.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://knt.vehdjk.com

[R66] 定时任务
来源：http://vgn.tanke756.top

crontab -e;  crontab -l
来源：http://pgu.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://wvz.cheryme.top

openssl rand -hex 16
来源：http://evj.ydjk.org.cn

[R68] 计算文件校验值
来源：http://dks.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://knv.gaohongyu789.top

[R69] 生成随机密码
来源：http://emh.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://trd.dianchejie.cn

[R70] 时间戳与互转
来源：http://gkx.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://ohy.nwbrower.top

[R71] 日期格式化
来源：http://myo.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xrx.zhiwuduotai.top

[R72] 等待端口就绪
来源：http://yop.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lok.yonumen.top

[R73] 分割大日志
来源：http://oje.zdbjq.cn

split -l 1000 big.log part_
来源：http://vfv.zhixingplan.top

[R74] 批量重命名
来源：http://mup.fktsv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ebi.ivvv.top

[R75] 导出环境变量
来源：http://hvq.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://vpw.316326.xyz

[R76] 使用临时文件
来源：http://bwm.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cvp.tian-w.cn

[R77] 读取用户输入
来源：http://fec.daria6918.cn

read -rp "请输入: " ans
来源：http://wnh.wangdashe.top

[R78] 交互式菜单
来源：http://ywq.uphjek.com

select opt in a b c; do echo "$opt"; break; done
来源：http://bfc.dianchejie.cn

[R79] 解析命令行选项
来源：http://xtj.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zzs.yj20258.top

[R80] 查看脚本执行耗时
来源：http://xns.hesvh.cn

time ./run.sh
来源：http://dnv.0kj1m.cn

================================================================================
来源：http://dtd.sxryk.cn

S. C / C++ 专题
来源：http://pov.hysaishi.cn

================================================================================
来源：http://apc.vqdsnc.cn

[S01] C：Hello World
来源：http://tjw.nanxuanxn.top

#include <stdio.h>
来源：http://nhy.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ogq.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://ksi.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://ngp.316326.xyz

[S03] C：读入整数
来源：http://gep.ehwqpu.com

int x; scanf("%d", &x);
来源：http://qzl.jyoumei.cn

[S04] C：字符串复制
来源：http://qyv.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://igi.ydjk.org.cn

[S05] C：字符串长度
来源：http://ywm.shanyushiyangtech.top

strlen(s)
来源：http://kuh.vqdsnc.cn

[S06] C：字符串比较
来源：http://yap.hcnkem.com

strcmp(a, b) == 0
来源：http://wmx.meibo888.top

[S07] C：数组遍历求和
来源：http://atq.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wij.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://ngh.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jer.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://yrk.316326.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://itd.ydjk.org.cn

[S10] C：指针与解引用
来源：http://shp.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://hjk.yueranfly.top

[S11] C：逐行读文件
来源：http://tew.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://ksi.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cvb.pengpengdd.cyou

fclose(f);
来源：http://qyr.yuxming.cn

[S12] C：写文件
来源：http://uwb.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ofn.jlsjyb.cn

[S13] C：宏定义
来源：http://lkv.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eod.nwbrower.top

[S14] C：枚举
来源：http://vos.fanxiaobao.xyz

enum Color { RED, GREEN, BLUE };
来源：http://asg.jinqigfzy.top

[S15] C：类型转换
来源：http://kpx.tanke756.top

(double) a / b
来源：http://ycc.pengpengdd.cyou

[S16] C：位操作置位
来源：http://wyr.meibo888.top

x |= (1 << 3);
来源：http://gxn.hammf.cn

[S17] C：安全拼接字符串
来源：http://iso.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fwh.ydjk.org.cn

[S18] C：命令行参数
来源：http://oja.cqqwz.cn

int main(int argc, char **argv)
来源：http://avp.yuxming.cn

[S19] C：快速排序
来源：http://inr.yuanzhike.top

qsort(a, n, sizeof(int), cmp);
来源：http://jhh.yuanzhike.top

[S20] C：二分查找
来源：http://hgd.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qaf.yonumen.top

[S21] C：字符类别判断
来源：http://rrt.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vhl.ydjk.org.cn

[S22] C：字符串转数字
来源：http://cmx.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lfo.hesvh.cn

[S23] C：随机数
来源：http://lzh.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ffp.epnwcf.com

[S24] C：获取本地时间
来源：http://uul.redwolf501.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uly.dashuyun.cn

[S25] C：内存拷贝
来源：http://qps.epnwcf.com

memcpy(dst, src, n);
来源：http://roq.ehwqpu.com

[S26] C：内存清零
来源：http://ybl.gogol.net.cn

memset(a, 0, sizeof a);
来源：http://jwy.hnxiangtu.top

[S27] C：定义常量
来源：http://ioe.svipenyu.cn

const double PI = 3.14159;
来源：http://jbb.jqgfzy.top

[S28] C：静态变量
来源：http://lmm.haohaochexian.top

static int counter = 0;
来源：http://rqw.nanxinkj.top

[S29] C：变参函数
来源：http://vyl.cucudq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lph.316326.xyz

[S30] C：头文件保护
来源：http://wtw.chenzaomai.com

#ifndef X_H
来源：http://fdi.xuetiantiany.cn

#define X_H
来源：http://dbl.zhoulong.xyz

#endif
来源：http://nci.xuetiantiany.cn

[S31] C++：Hello World
来源：http://yom.yj20258.top

#include <iostream>
来源：http://ksm.cdnleiting.top

int main() { std::cout << "Hello\n"; }
来源：http://gur.daxiang520.top

[S32] C++：字符串
来源：http://asf.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://oiv.yangfankeji.com

[S33] C++：vector 增删
来源：http://dem.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oxd.ivvv.top

[S34] C++：遍历 vector
来源：http://ifq.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://eey.redwolf501.top

[S35] C++：map
来源：http://mmk.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vjo.wangdashe.top

[S36] C++：unordered_map
来源：http://jbg.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rls.316326.xyz

[S37] C++：set
来源：http://iwo.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://itu.cucudq.cn

[S38] C++：排序
来源：http://bcr.52xcode.cn

std::sort(v.begin(), v.end());
来源：http://cds.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://amk.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nqt.zhijiandao.cn

[S40] C++：查找元素
来源：http://uld.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tde.wangshuangyany.cn

[S41] C++：类与构造函数
来源：http://ijs.svipenyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tco.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://jhf.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://cte.uphjek.com

[S43] C++：智能指针
来源：http://lgr.sysykeji.top

auto p = std::make_unique<int>(5);
来源：http://amp.gaohongyu789.top

[S44] C++：引用传参
来源：http://msp.cheryme.top

void inc(int &x) { ++x; }
来源：http://mgg.smart0.xyz

[S45] C++：lambda
来源：http://zlr.xingfuxueyuan.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://dlh.chenjidiqi.icu

[S46] C++：函数模板
来源：http://bcd.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nnq.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://qws.zhijiandao.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qtw.yuanzhike.top

[S48] C++：逐行读文件
来源：http://bhw.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://ppl.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://lle.tarul.cn

[S49] C++：写文件
来源：http://xxe.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bpv.bjfxy.top

[S50] C++：格式化数字
来源：http://vii.tarul.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wmu.guowangkeji.top

[S51] C++：显式类型转换
来源：http://dao.pycfn.com

static_cast<double>(a) / b
来源：http://ptq.zdqjudy.top

[S52] C++：const 与 noexcept
来源：http://fuv.sweek.top

int size() const noexcept { return n_; }
来源：http://znj.sysykeji.top

[S53] C++：移动语义
来源：http://upr.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://iiq.vqdsnc.cn

[S54] C++：异常处理
来源：http://kzj.nanxuanxn.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gum.cheryme.top

[S55] C++：结构化绑定
来源：http://hiy.wangshuangyany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rct.jinqigufen.top

[S56] C++：optional
来源：http://qmi.jinghuilouyu.cn


<!-- 参考信息 -->