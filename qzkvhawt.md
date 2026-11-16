代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://uvt.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://npb.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fpl.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://lmg.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vip.zhengqikj.top

[Q90] 生成序号列
来源：http://kwa.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eam.jinqigfzy.top

================================================================================
来源：http://kyn.jinyuanbaomall.cn

R. Bash 专题
来源：http://kil.nanxuanxn.top

================================================================================
来源：http://wdu.sysykeji.top

[R01] shebang 与严格模式
来源：http://dzj.dianchejie.cn

#!/usr/bin/env bash
来源：http://dlc.zhaomingkeji.xyz

set -euo pipefail
来源：http://cxr.zhixingplan.top

[R02] 变量赋值与使用
来源：http://ccr.yj20258.top

name="Tom"; echo "$name"
来源：http://ujj.nanxinkj.top

[R03] 只读变量
来源：http://bvv.zycfv.cn

readonly PI=3.14
来源：http://pwi.hongshengwenyu.top

[R04] 位置参数
来源：http://ehg.ywan-chungtsiang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kym.yanxiufei.cn

[R05] 参数默认值
来源：http://rlo.chenjidiqi.icu

name="${1:-default}"
来源：http://mxg.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://tcs.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yim.yuanzhike.top

[R07] if 判断文件
来源：http://esg.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mqu.sweek.top

[R08] 数值比较
来源：http://kkx.fanxiaobao.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://dkk.316326.xyz

[R09] 字符串比较
来源：http://hvl.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://btr.birdmap.top

[R10] 正则匹配
来源：http://uvz.sxryk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bhv.pycfn.com

[R11] case 多分支
来源：http://iar.aizwys.cn

case "$1" in
来源：http://roo.redwolf501.top

start) echo "启动" ;;
来源：http://dbg.havefunace.top

stop)  echo "停止" ;;
来源：http://jgd.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://qht.iojbl.cn

esac
来源：http://xch.dianchejie.cn

[R12] for 遍历文件
来源：http://saa.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://iqz.zhiwuduotai.top

[R13] for 计数循环
来源：http://unp.0kj1m.cn

for i in {1..10}; do echo "$i"; done
来源：http://vqs.ivvv.top

[R14] C 风格 for
来源：http://mkh.meibo888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uoo.cucudq.cn

[R15] while 逐行读文件
来源：http://oky.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://grt.shanyushiyangtech.top

[R16] until 等待条件
来源：http://wtw.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fll.chenjidiqi.icu

[R17] 数组定义与取值
来源：http://gyj.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://znk.epnwcf.com

[R18] 遍历数组
来源：http://ydq.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ssv.chenzaomai.com

[R19] 数组长度
来源：http://mok.shanyushiyangkeji.top

echo "${#arr[@]}"
来源：http://nyq.svipenyu.cn

[R20] 关联数组（字典）
来源：http://tbv.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aak.iojbl.cn

[R21] 字符串长度
来源：http://dqr.52xcode.cn

echo "${#s}"
来源：http://ckt.kuanghao11.cn

[R22] 截取子串
来源：http://xlo.tanke756.top

echo "${s:0:5}"
来源：http://itp.dashuyun.cn

[R23] 字符串替换
来源：http://lfd.daria6918.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ktd.yonumen.top

[R24] 大小写转换
来源：http://clg.zhixingplan.top

echo "${s^^}"; echo "${s,,}"
来源：http://nhn.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://oah.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gem.zdbjq.cn

[R26] 命令替换
来源：http://ypg.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://ijv.jyoumei.cn

[R27] 算术展开
来源：http://dns.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://prl.nanxinkj.top

[R28] 浮点运算
来源：http://feg.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://mdb.ywan-chungtsiang.top

[R29] 定义函数
来源：http://ojo.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ztb.vehdjk.com

[R30] 函数返回状态码
来源：http://and.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://xll.andypj.xyz

[R31] 局部变量
来源：http://qzx.0kj1m.cn

f() { local x=1; echo "$x"; }
来源：http://ojf.hcnkem.com

[R32] 参数个数校验
来源：http://yrc.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bmk.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://tfk.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wdw.bjfxy.top

[R34] 退出时清理
来源：http://qet.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nrg.aizwys.cn

[R35] 后台执行并等待
来源：http://boz.gotoacloud.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ykv.0kj1m.cn

[R36] 并发执行多个任务
来源：http://qex.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://luj.havefunace.top

[R37] 把输出赋给变量
来源：http://nxf.jqgufenzy.top

files=$(ls -1)
来源：http://hek.shanyushiyangkeji.top

[R38] 管道串联
来源：http://uyx.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://nke.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://mmy.zhijiandao.cn

cmd > out.log 2>&1
来源：http://esn.pengpengdd.cyou

[R40] 追加写日志
来源：http://qgu.zhoulong.xyz

echo "log" >> out.log
来源：http://wqu.sweek.top

[R41] 丢弃输出
来源：http://kux.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://env.zhoulong.xyz

[R42] 输入重定向
来源：http://vrg.cucudq.cn

wc -l < a.txt
来源：http://xur.andypj.xyz

[R43] 按名字查找文件
来源：http://dxi.hcnkem.com

find . -name "*.log" -type f
来源：http://gbi.epnwcf.com

[R44] 按修改时间查找
来源：http://ida.haohaochexian.top

find . -mtime -7 -type f
来源：http://zxj.xinyue.icu

[R45] 批量删除
来源：http://xgy.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://xbb.haohaochexian.top

[R46] 递归替换文件内容
来源：http://iti.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qov.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://dwj.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://lhi.xingfuxueyuan.xyz

[R48] awk 取指定列
来源：http://vmc.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://mdr.wangdashe.top

[R49] awk 带条件
来源：http://phb.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vpq.yuanzhike.top

[R50] awk 求和
来源：http://eux.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://auv.jqgfzy.top

[R51] 排序去重取前几
来源：http://saq.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://epl.nwbrower.top

[R52] 统计行数
来源：http://wbf.daria6918.cn

wc -l a.txt
来源：http://bsi.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://uib.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bpl.uphjek.com

[R54] 比较两个文件
来源：http://cvr.tian-w.cn

diff a.txt b.txt
来源：http://jcf.hysaishi.cn

[R55] 压缩与解压
来源：http://zdm.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zzh.yangfankeji.com

[R56] 远程拷贝
来源：http://leq.gzhubu.top

scp file user@host:/path/
来源：http://nmt.dashuyun.cn

[R57] 远程执行命令
来源：http://ezi.andypj.xyz

ssh user@host 'uptime'
来源：http://mqn.jqgufenzy.top

[R58] 下载文件
来源：http://cza.shanyushiyangtech.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bjp.jiagoushi.top

[R59] 发 POST JSON
来源：http://mje.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nkk.daria6918.cn

[R60] 只看 HTTP 状态码
来源：http://ghh.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://npp.yfazqb.com

[R61] 磁盘占用
来源：http://fbr.jianghu66.top

df -h;  du -sh *
来源：http://bep.daria6918.cn

[R62] 找最占空间的文件
来源：http://mcf.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://xkx.dianchejie.cn

[R63] 内存与进程
来源：http://mxf.yuanzhike.top

free -h;  ps aux | grep nginx
来源：http://dgw.yvedp.cn

[R64] 结束进程
来源：http://hti.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://ren.smart0.xyz

[R65] 查看端口占用
来源：http://svc.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lnu.jyoumei.cn

[R66] 定时任务
来源：http://cxx.tian-w.cn

crontab -e;  crontab -l
来源：http://jrg.andypj.xyz

[R67] 生成随机十六进制串
来源：http://xdq.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://kml.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://fvt.quarkkingdee.top

sha256sum a.txt;  md5sum a.txt
来源：http://xzb.jinqigfzy.top

[R69] 生成随机密码
来源：http://ldi.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://zws.uphjek.com

[R70] 时间戳与互转
来源：http://tgk.tanke756.top

date +%s;  date -d @1700000000
来源：http://sdd.jiagoushi.top

[R71] 日期格式化
来源：http://fdy.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ifn.jiagoushi.top

[R72] 等待端口就绪
来源：http://gag.yvedp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qki.zhixingplan.top

[R73] 分割大日志
来源：http://hds.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://cjx.yuanzhike.top

[R74] 批量重命名
来源：http://pux.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eeo.svipenyu.cn

[R75] 导出环境变量
来源：http://jbd.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://ehz.cheryme.top

[R76] 使用临时文件
来源：http://mws.havefunace.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rih.ppjwa.cn

[R77] 读取用户输入
来源：http://qor.jyoumei.cn

read -rp "请输入: " ans
来源：http://rha.bjfxy.top

[R78] 交互式菜单
来源：http://hok.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rgp.yuxming.cn

[R79] 解析命令行选项
来源：http://bsc.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qqp.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://hom.andypj.xyz

time ./run.sh
来源：http://vim.jianghu66.top

================================================================================
来源：http://blg.yj202588.top

S. C / C++ 专题
来源：http://yuc.shzxlz.cn

================================================================================
来源：http://zui.wangshuangyany.cn

[S01] C：Hello World
来源：http://rte.xziqi.cn

#include <stdio.h>
来源：http://vzf.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cyh.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://oxa.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://utl.sufxvd.cn

[S03] C：读入整数
来源：http://tjy.xziqi.cn

int x; scanf("%d", &x);
来源：http://aho.andypj.xyz

[S04] C：字符串复制
来源：http://pnp.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tpo.vqdsnc.cn

[S05] C：字符串长度
来源：http://vsp.meibo888.top

strlen(s)
来源：http://bux.zdqjudy.top

[S06] C：字符串比较
来源：http://jfx.hysaishi.cn

strcmp(a, b) == 0
来源：http://qkn.snrcjt.cn

[S07] C：数组遍历求和
来源：http://akl.yonumen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vmo.chenjidiqi.icu

[S08] C：动态内存分配与释放
来源：http://zda.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lpo.zhengqikj.top

[S09] C：结构体定义与初始化
来源：http://div.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fab.yonumen.top

[S10] C：指针与解引用
来源：http://zbo.yj20258888.top

int *p = &a;  *p = 5;
来源：http://jug.c1oappe.top

[S11] C：逐行读文件
来源：http://ipt.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://wek.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ytq.zhoulong.xyz

fclose(f);
来源：http://mxp.chenlongwang.top

[S12] C：写文件
来源：http://wtl.redwolf501.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uie.gogol.net.cn

[S13] C：宏定义
来源：http://dwo.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fxr.0kj1m.cn

[S14] C：枚举
来源：http://pfk.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://ika.yvedp.cn

[S15] C：类型转换
来源：http://iiw.aibaodan.cn

(double) a / b
来源：http://wnq.tian-w.cn

[S16] C：位操作置位
来源：http://cds.sysykeji.top

x |= (1 << 3);
来源：http://ihe.guannengcc.top

[S17] C：安全拼接字符串
来源：http://fzf.cqqwz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ofl.sysykeji.top

[S18] C：命令行参数
来源：http://uel.aizwys.cn

int main(int argc, char **argv)
来源：http://wgr.daxiang520.top

[S19] C：快速排序
来源：http://ktl.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zxm.hfpthk.cn

[S20] C：二分查找
来源：http://mib.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ooa.jiagoushi.top

[S21] C：字符类别判断
来源：http://xsa.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jgu.yj202588.top

[S22] C：字符串转数字
来源：http://wgl.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://brj.cqqwz.cn

[S23] C：随机数
来源：http://fhe.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fue.52xcode.cn

[S24] C：获取本地时间
来源：http://dih.yanxiufei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kqh.yuanzhike.top

[S25] C：内存拷贝
来源：http://fwo.havefunace.top

memcpy(dst, src, n);
来源：http://apj.zhongyouzk.top

[S26] C：内存清零
来源：http://cvo.fengsongda.top

memset(a, 0, sizeof a);
来源：http://tqk.ivvv.top

[S27] C：定义常量
来源：http://uct.ydzc1.top

const double PI = 3.14159;
来源：http://iox.birdmap.top

[S28] C：静态变量
来源：http://umi.chenzaomai.com

static int counter = 0;
来源：http://nly.cashguo.top

[S29] C：变参函数
来源：http://grh.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ceb.kuanghao11.cn

[S30] C：头文件保护
来源：http://svl.nanxuanxn.top

#ifndef X_H
来源：http://vad.gotoacloud.top

#define X_H
来源：http://wcy.andypj.xyz

#endif
来源：http://uzv.hywenlv.cn

[S31] C++：Hello World
来源：http://pnz.sxryk.cn

#include <iostream>
来源：http://xnw.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://fgq.shanyushiyangkeji.top

[S32] C++：字符串
来源：http://lvj.fanxiaobao.xyz

std::string s = "hi";  s += "!";
来源：http://awt.cheryme.top

[S33] C++：vector 增删
来源：http://btd.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qwk.yongpay.top

[S34] C++：遍历 vector
来源：http://aob.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://bsc.hongshengwenyu.top

[S35] C++：map
来源：http://aki.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ixu.hysaishi.cn

[S36] C++：unordered_map
来源：http://udu.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wet.shzxlz.cn

[S37] C++：set
来源：http://hjr.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://caf.fengsongda.top

[S38] C++：排序
来源：http://rdt.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://ayu.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://ekl.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ymg.xylfe.cn

[S40] C++：查找元素
来源：http://trq.aizwys.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ixi.shanyushiyangtech.top

[S41] C++：类与构造函数
来源：http://hty.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cjm.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://xla.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://yui.jinqigfzy.top

[S43] C++：智能指针
来源：http://nuh.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://hmy.vehdjk.com

[S44] C++：引用传参
来源：http://ixc.yj202588.top

void inc(int &x) { ++x; }
来源：http://ixc.sjlbkw.cn

[S45] C++：lambda
来源：http://lup.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://pxw.chenzaomai.com

[S46] C++：函数模板
来源：http://qrq.haohaochexian.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pqi.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://gpx.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qel.hcnkem.com

[S48] C++：逐行读文件
来源：http://byr.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://roq.snrcjt.cn

while (std::getline(in, line)) { }
来源：http://gjg.c1oappe.top

[S49] C++：写文件
来源：http://jyk.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hhe.jiagoushi.top

[S50] C++：格式化数字
来源：http://uud.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vdb.cheryme.top

[S51] C++：显式类型转换
来源：http://kwi.hysaishi.cn

static_cast<double>(a) / b
来源：http://pjx.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://fei.sweek.top

int size() const noexcept { return n_; }
来源：http://rtn.jqgfzy.top

[S53] C++：移动语义
来源：http://fyo.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://bea.yanxiufei.cn

[S54] C++：异常处理
来源：http://mmv.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zuu.gogol.net.cn

[S55] C++：结构化绑定
来源：http://nse.bjfxy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bcn.zdqjudy.top

[S56] C++：optional
来源：http://qcx.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lje.snrcjt.cn

[S57] C++：编译期常量
来源：http://lwn.mhx1999.top

constexpr int N = 10;
来源：http://pks.316326.xyz

[S58] C++：命名空间
来源：http://vpt.jianghu66.top


<!-- 参考信息 -->