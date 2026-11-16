代发 wailian999

[Q86] 读取 JSON 字段
来源：http://zpw.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://plt.daxiang520.top

[Q87] JSON 字段做条件
来源：http://vhm.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jzd.xuanzx.com

[Q88] 行转列（条件聚合）
来源：http://yho.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bmj.birdmap.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eja.zycfv.cn

[Q89] 判断表是否存在
来源：http://cqn.nanxuanxn.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lcl.shanyushiyangkeji.top

[Q90] 生成序号列
来源：http://sss.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vjd.aibaodan.cn

================================================================================
来源：http://vdy.sweek.top

R. Bash 专题
来源：http://cvr.bbcook.cn

================================================================================
来源：http://ccr.xylfe.cn

[R01] shebang 与严格模式
来源：http://nko.hnxiangtu.top

#!/usr/bin/env bash
来源：http://hmu.chenzaomai.com

set -euo pipefail
来源：http://epi.zhengqikj.top

[R02] 变量赋值与使用
来源：http://vby.xinyue.icu

name="Tom"; echo "$name"
来源：http://ifo.sweek.top

[R03] 只读变量
来源：http://mqc.xylfe.cn

readonly PI=3.14
来源：http://dmv.hcnkem.com

[R04] 位置参数
来源：http://xbv.ydjk.org.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tuq.fzhhl.top

[R05] 参数默认值
来源：http://ome.fzhhl.top

name="${1:-default}"
来源：http://hgy.zhixingplan.top

[R06] 判断命令是否存在
来源：http://dll.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ajh.hysaishi.cn

[R07] if 判断文件
来源：http://qaw.yj202588.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pdf.ppjwa.cn

[R08] 数值比较
来源：http://rop.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wdy.dianchejie.cn

[R09] 字符串比较
来源：http://sdz.mhx1999.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wqw.vqdsnc.cn

[R10] 正则匹配
来源：http://vak.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rja.ehwqpu.com

[R11] case 多分支
来源：http://opa.chenjidiqi.icu

case "$1" in
来源：http://epz.fzhhl.top

start) echo "启动" ;;
来源：http://ztu.kuanghao11.cn

stop)  echo "停止" ;;
来源：http://txq.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://cjn.ehwqpu.com

esac
来源：http://sig.bbcook.cn

[R12] for 遍历文件
来源：http://ahs.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://rzr.sweek.top

[R13] for 计数循环
来源：http://ziw.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://pvl.zhengqikj.top

[R14] C 风格 for
来源：http://ysy.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ybh.andypj.xyz

[R15] while 逐行读文件
来源：http://zfm.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pfi.cheryme.top

[R16] until 等待条件
来源：http://thl.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zrr.quarkkingdee.top

[R17] 数组定义与取值
来源：http://qxy.quarkkingdee.top

arr=(a b c); echo "${arr[0]}"
来源：http://oxm.yueranfly.top

[R18] 遍历数组
来源：http://lqq.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://scj.feifeiyinyue.top

[R19] 数组长度
来源：http://vod.hongshengwenyu.top

echo "${#arr[@]}"
来源：http://mjc.shuidangran.top

[R20] 关联数组（字典）
来源：http://kpz.vqdsnc.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zva.gzhubu.top

[R21] 字符串长度
来源：http://vzs.zhixingplan.top

echo "${#s}"
来源：http://jbr.jqgfzy.top

[R22] 截取子串
来源：http://ppk.xylfe.cn

echo "${s:0:5}"
来源：http://syu.yangfankeji.com

[R23] 字符串替换
来源：http://ljm.dashuyun.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dty.yanxiufei.cn

[R24] 大小写转换
来源：http://fes.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://jen.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://kxh.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://juj.guannengcc.top

[R26] 命令替换
来源：http://amp.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://ink.cheryme.top

[R27] 算术展开
来源：http://rae.nwbrower.top

echo $((1 + 2 * 3))
来源：http://vnq.ivvv.top

[R28] 浮点运算
来源：http://rqm.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://bnk.yvedp.cn

[R29] 定义函数
来源：http://xso.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mzl.havefunace.top

[R30] 函数返回状态码
来源：http://edv.gogol.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://kcw.guowangkeji.top

[R31] 局部变量
来源：http://haj.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://ult.bjfxy.top

[R32] 参数个数校验
来源：http://ozq.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fon.jqgufenzy.top

[R33] 捕获错误并提示行号
来源：http://rte.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lir.zhongyouzk.top

[R34] 退出时清理
来源：http://jkh.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://gok.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://fwl.ehwqpu.com

sleep 5 & pid=$!; wait "$pid"
来源：http://faa.hcnkem.com

[R36] 并发执行多个任务
来源：http://wga.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://adn.fehbvm.com

[R37] 把输出赋给变量
来源：http://ltn.jlsjyb.cn

files=$(ls -1)
来源：http://bwd.fehbvm.com

[R38] 管道串联
来源：http://agk.jiagoushi.top

cat a.txt | grep -i error | wc -l
来源：http://zyd.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://wve.fehbvm.com

cmd > out.log 2>&1
来源：http://bkd.andypj.xyz

[R40] 追加写日志
来源：http://aad.pycfn.com

echo "log" >> out.log
来源：http://rhu.andypj.xyz

[R41] 丢弃输出
来源：http://voh.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://yzz.jianghu66.top

[R42] 输入重定向
来源：http://tcq.zycfv.cn

wc -l < a.txt
来源：http://zdt.ydzc1.top

[R43] 按名字查找文件
来源：http://kww.jinqigfzy.top

find . -name "*.log" -type f
来源：http://rxo.dashuyun.cn

[R44] 按修改时间查找
来源：http://drj.meibo888.top

find . -mtime -7 -type f
来源：http://syb.aibaodan.cn

[R45] 批量删除
来源：http://cmy.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://dcm.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://dfx.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zdy.sweek.top

[R47] sed 单行替换
来源：http://czh.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://xba.xingfuxueyuan.xyz

[R48] awk 取指定列
来源：http://yiy.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://lld.sufxvd.cn

[R49] awk 带条件
来源：http://ggb.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zvv.xylfe.cn

[R50] awk 求和
来源：http://uqb.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://lnp.yongpay.top

[R51] 排序去重取前几
来源：http://suq.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lay.snrcjt.cn

[R52] 统计行数
来源：http://zaw.yj20258.top

wc -l a.txt
来源：http://qpr.tianlin.xyz

[R53] 查看文件头与实时尾
来源：http://rna.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://grh.aizwys.cn

[R54] 比较两个文件
来源：http://zzd.shzxlz.cn

diff a.txt b.txt
来源：http://ozu.jyoumei.cn

[R55] 压缩与解压
来源：http://vcc.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jze.dashuyun.cn

[R56] 远程拷贝
来源：http://mck.jinqigufen.top

scp file user@host:/path/
来源：http://hfx.nwbrower.top

[R57] 远程执行命令
来源：http://nmy.c1oappe.top

ssh user@host 'uptime'
来源：http://ozv.guannengcc.top

[R58] 下载文件
来源：http://oop.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tqt.chenzaomai.com

[R59] 发 POST JSON
来源：http://eud.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vwf.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://jny.316326.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hyv.bbcook.cn

[R61] 磁盘占用
来源：http://bty.ydjk.org.cn

df -h;  du -sh *
来源：http://zwl.bbcook.cn

[R62] 找最占空间的文件
来源：http://ncp.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://pav.shanyushiyangkeji.top

[R63] 内存与进程
来源：http://nms.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://eob.sysykeji.top

[R64] 结束进程
来源：http://pop.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://ymc.bbcook.cn

[R65] 查看端口占用
来源：http://hzr.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mhv.meibo888.top

[R66] 定时任务
来源：http://bxo.shzxlz.cn

crontab -e;  crontab -l
来源：http://wwb.gzhubu.top

[R67] 生成随机十六进制串
来源：http://ryr.quarkkingdee.top

openssl rand -hex 16
来源：http://zgc.gzhubu.top

[R68] 计算文件校验值
来源：http://njc.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://uwg.zhoulong.xyz

[R69] 生成随机密码
来源：http://vdd.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://dvh.sxryk.cn

[R70] 时间戳与互转
来源：http://ael.jlsjyb.cn

date +%s;  date -d @1700000000
来源：http://mvx.fanxiaobao.xyz

[R71] 日期格式化
来源：http://kam.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nat.cashguo.top

[R72] 等待端口就绪
来源：http://fng.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rwj.iojbl.cn

[R73] 分割大日志
来源：http://gqp.yj202588.top

split -l 1000 big.log part_
来源：http://nrm.zycfv.cn

[R74] 批量重命名
来源：http://kyz.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vcp.hnxiangtu.top

[R75] 导出环境变量
来源：http://hqs.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://baj.wangdashe.top

[R76] 使用临时文件
来源：http://wlv.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fyv.guowangkeji.top

[R77] 读取用户输入
来源：http://xpm.yongpay.top

read -rp "请输入: " ans
来源：http://fom.chenjidiqi.icu

[R78] 交互式菜单
来源：http://vks.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jjl.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://iwz.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gev.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://ham.gogol.net.cn

time ./run.sh
来源：http://gcs.yuxming.cn

================================================================================
来源：http://eyc.chenzaomai.com

S. C / C++ 专题
来源：http://cgx.yvedp.cn

================================================================================
来源：http://anz.uphjek.com

[S01] C：Hello World
来源：http://iam.chenlongwang.top

#include <stdio.h>
来源：http://vhb.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://snb.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://oyi.chenzaomai.com

int a = 10; printf("%d\n", a);
来源：http://uuw.dianchejie.cn

[S03] C：读入整数
来源：http://vmx.xinyue.icu

int x; scanf("%d", &x);
来源：http://owm.yfazqb.com

[S04] C：字符串复制
来源：http://kdk.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://yvx.chenlongwang.top

[S05] C：字符串长度
来源：http://upx.hfpthk.cn

strlen(s)
来源：http://hgk.vehdjk.com

[S06] C：字符串比较
来源：http://rcb.andypj.xyz

strcmp(a, b) == 0
来源：http://wmp.0kj1m.cn

[S07] C：数组遍历求和
来源：http://mdi.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tha.jyoumei.cn

[S08] C：动态内存分配与释放
来源：http://zpv.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qqv.yuxming.cn

[S09] C：结构体定义与初始化
来源：http://egx.feifeiyinyue.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ccf.yanxiufei.cn

[S10] C：指针与解引用
来源：http://cjw.jinqigufen.top

int *p = &a;  *p = 5;
来源：http://lfk.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://yre.yueranfly.top

FILE *f = fopen("a.txt", "r");
来源：http://sem.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bkn.yj202588.top

fclose(f);
来源：http://neo.jlsjyb.cn

[S12] C：写文件
来源：http://zxa.cucudq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rce.haohaochexian.top

[S13] C：宏定义
来源：http://jqb.jianghu66.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nmm.ehwqpu.com

[S14] C：枚举
来源：http://nos.yj202588.top

enum Color { RED, GREEN, BLUE };
来源：http://jul.fengsongda.top

[S15] C：类型转换
来源：http://xuz.nanxuanxn.top

(double) a / b
来源：http://azv.yueranfly.top

[S16] C：位操作置位
来源：http://tmr.hongshengwenyu.top

x |= (1 << 3);
来源：http://jpr.nwbrower.top

[S17] C：安全拼接字符串
来源：http://gqi.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gpt.bbcook.cn

[S18] C：命令行参数
来源：http://mhf.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://tsu.bjfxy.top

[S19] C：快速排序
来源：http://grj.nwbrower.top

qsort(a, n, sizeof(int), cmp);
来源：http://myn.hfpthk.cn

[S20] C：二分查找
来源：http://thq.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sns.guannengcc.top

[S21] C：字符类别判断
来源：http://jfx.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tsj.c1oappe.top

[S22] C：字符串转数字
来源：http://zjh.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xbi.snrcjt.cn

[S23] C：随机数
来源：http://xxl.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zxo.nanxuanxn.top

[S24] C：获取本地时间
来源：http://okl.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bza.aizwys.cn

[S25] C：内存拷贝
来源：http://scs.gaohongyu789.top

memcpy(dst, src, n);
来源：http://xeo.ppjwa.cn

[S26] C：内存清零
来源：http://jcg.hcnkem.com

memset(a, 0, sizeof a);
来源：http://owb.yuxming.cn

[S27] C：定义常量
来源：http://kxk.hfpthk.cn

const double PI = 3.14159;
来源：http://qfx.zhengqikj.top

[S28] C：静态变量
来源：http://aed.redwolf501.top

static int counter = 0;
来源：http://mue.shangyingyoupin.top

[S29] C：变参函数
来源：http://yph.yangfankeji.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://enc.xinyue.icu

[S30] C：头文件保护
来源：http://kiu.ydzc1.top

#ifndef X_H
来源：http://cde.hnqzz.top

#define X_H
来源：http://vxi.gaohongyu789.top

#endif
来源：http://xus.yonumen.top

[S31] C++：Hello World
来源：http://bgz.jqgufenzy.top

#include <iostream>
来源：http://ers.chenzaomai.com

int main() { std::cout << "Hello\n"; }
来源：http://hji.andypj.xyz

[S32] C++：字符串
来源：http://eht.cashguo.top

std::string s = "hi";  s += "!";
来源：http://pad.yanxiufei.cn

[S33] C++：vector 增删
来源：http://wvl.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hwx.zycfv.cn

[S34] C++：遍历 vector
来源：http://eby.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://xnz.nanxinkj.top

[S35] C++：map
来源：http://hjl.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mwi.gogol.net.cn

[S36] C++：unordered_map
来源：http://ppx.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wjd.yongpay.top

[S37] C++：set
来源：http://dem.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ciq.pycfn.com

[S38] C++：排序
来源：http://dvg.pycfn.com

std::sort(v.begin(), v.end());
来源：http://jia.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://xwm.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uul.xuetiantiany.cn

[S40] C++：查找元素
来源：http://tqe.fanxiaobao.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mln.sysykeji.top

[S41] C++：类与构造函数
来源：http://moc.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kra.bjfxy.top

[S42] C++：继承与虚函数
来源：http://sim.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://xpz.zhijiandao.cn

[S43] C++：智能指针
来源：http://eol.fktsv.cn

auto p = std::make_unique<int>(5);
来源：http://gfr.meibo888.top

[S44] C++：引用传参
来源：http://xux.chenlongwang.top

void inc(int &x) { ++x; }
来源：http://zyt.sxryk.cn

[S45] C++：lambda
来源：http://uie.pengpengdd.cyou

auto add = [](int a, int b) { return a + b; };
来源：http://imw.gaohongyu789.top

[S46] C++：函数模板
来源：http://zor.hnqzz.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://glu.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://see.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gqv.daxiang520.top

[S48] C++：逐行读文件
来源：http://ryt.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://mtd.jinghuilouyu.cn

while (std::getline(in, line)) { }
来源：http://fnx.fanxiaobao.xyz

[S49] C++：写文件
来源：http://dmk.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rkr.andypj.xyz

[S50] C++：格式化数字
来源：http://swl.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oop.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://gqx.hesvh.cn

static_cast<double>(a) / b
来源：http://iyl.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://xig.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://idp.c1oappe.top

[S53] C++：移动语义
来源：http://jcp.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://rrd.dashuyun.cn

[S54] C++：异常处理
来源：http://ygr.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://glh.gzhubu.top

[S55] C++：结构化绑定
来源：http://xfp.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cuc.dianchejie.cn

[S56] C++：optional
来源：http://hef.uphjek.com


<!-- 参考信息 -->