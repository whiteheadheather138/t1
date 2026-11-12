代发 wailian999

[Q84] 去除首尾空格
来源：http://mhm.xziqi.cn

SELECT TRIM(name) FROM users;
来源：http://fml.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://xuw.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ogd.sjlbkw.cn

[Q86] 读取 JSON 字段
来源：http://vxr.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ybp.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://btg.52xcode.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fxw.birdmap.top

[Q88] 行转列（条件聚合）
来源：http://dea.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fxw.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yqy.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://ohc.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hjv.epnwcf.com

[Q90] 生成序号列
来源：http://rsq.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ofu.cdnleiting.top

================================================================================
来源：http://xzl.pycfn.com

R. Bash 专题
来源：http://lpq.gzhubu.top

================================================================================
来源：http://dhx.zdqjudy.top

[R01] shebang 与严格模式
来源：http://jju.jyoumei.cn

#!/usr/bin/env bash
来源：http://vgs.mhx1999.top

set -euo pipefail
来源：http://boh.xuanzx.com

[R02] 变量赋值与使用
来源：http://ztn.tianlin.xyz

name="Tom"; echo "$name"
来源：http://fmm.guowangkeji.top

[R03] 只读变量
来源：http://fqm.wangshuangyany.cn

readonly PI=3.14
来源：http://vjd.jqgufenzy.top

[R04] 位置参数
来源：http://ziy.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vta.zdqjudy.top

[R05] 参数默认值
来源：http://vnu.zhixingplan.top

name="${1:-default}"
来源：http://xxq.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://kvr.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vpj.yongpay.top

[R07] if 判断文件
来源：http://kpv.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://drm.quarkkingdee.top

[R08] 数值比较
来源：http://bdz.bjfxy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qjs.uphjek.com

[R09] 字符串比较
来源：http://vqy.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ugs.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://nea.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tys.hongshengwenyu.top

[R11] case 多分支
来源：http://ynm.meibo888.top

case "$1" in
来源：http://neo.ppjwa.cn

start) echo "启动" ;;
来源：http://pfj.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://nbg.jyoumei.cn

*)     echo "未知命令" ;;
来源：http://kbc.hfpthk.cn

esac
来源：http://ber.gogol.net.cn

[R12] for 遍历文件
来源：http://erd.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://vzj.yuanzhike.top

[R13] for 计数循环
来源：http://rdp.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://xwc.yj20258888.top

[R14] C 风格 for
来源：http://guf.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lim.tarul.cn

[R15] while 逐行读文件
来源：http://tag.redwolf501.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yye.sysykeji.top

[R16] until 等待条件
来源：http://uiv.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://amh.chenlongwang.top

[R17] 数组定义与取值
来源：http://gjw.shzxlz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://obd.fzhhl.top

[R18] 遍历数组
来源：http://kfx.yangfankeji.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vwh.cashguo.top

[R19] 数组长度
来源：http://ubk.xuanzx.com

echo "${#arr[@]}"
来源：http://oew.zdbjq.cn

[R20] 关联数组（字典）
来源：http://uai.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xmr.yuxming.cn

[R21] 字符串长度
来源：http://kff.jinqigfzy.top

echo "${#s}"
来源：http://duu.yj20258888.top

[R22] 截取子串
来源：http://jlz.gzhubu.top

echo "${s:0:5}"
来源：http://jkr.birdmap.top

[R23] 字符串替换
来源：http://sin.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jhn.tarul.cn

[R24] 大小写转换
来源：http://bxk.zdbjq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://frh.xylfe.cn

[R25] 去后缀 / 去前缀
来源：http://loe.cdnleiting.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://frw.shzxlz.cn

[R26] 命令替换
来源：http://nzd.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://ify.zhiwuduotai.top

[R27] 算术展开
来源：http://fmv.hnxiangtu.top

echo $((1 + 2 * 3))
来源：http://ybp.jinyuanbaomall.cn

[R28] 浮点运算
来源：http://vqi.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://oou.cqqwz.cn

[R29] 定义函数
来源：http://vfs.yueranfly.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qvd.52xcode.cn

[R30] 函数返回状态码
来源：http://ltg.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://tuw.yj20258888.top

[R31] 局部变量
来源：http://fqf.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://adb.bbcook.cn

[R32] 参数个数校验
来源：http://tro.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://spk.guowangkeji.top

[R33] 捕获错误并提示行号
来源：http://osg.kuanghao11.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fif.zhongyouzk.top

[R34] 退出时清理
来源：http://cdk.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://dgv.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://ouf.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ozn.hnqzz.top

[R36] 并发执行多个任务
来源：http://xmd.haohaochexian.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sbn.zdqjudy.top

[R37] 把输出赋给变量
来源：http://bqu.tian-w.cn

files=$(ls -1)
来源：http://wla.fktsv.cn

[R38] 管道串联
来源：http://vjf.0kj1m.cn

cat a.txt | grep -i error | wc -l
来源：http://bpo.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://hfv.nanxuanxn.top

cmd > out.log 2>&1
来源：http://zeu.sxryk.cn

[R40] 追加写日志
来源：http://qvb.chenjidiqi.icu

echo "log" >> out.log
来源：http://mxv.tarul.cn

[R41] 丢弃输出
来源：http://ydt.zycfv.cn

cmd >/dev/null 2>&1
来源：http://dkl.zhoulong.xyz

[R42] 输入重定向
来源：http://qdl.nanxinkj.top

wc -l < a.txt
来源：http://iuk.ydjk.org.cn

[R43] 按名字查找文件
来源：http://php.cqqwz.cn

find . -name "*.log" -type f
来源：http://mdt.zdbjq.cn

[R44] 按修改时间查找
来源：http://sih.316326.xyz

find . -mtime -7 -type f
来源：http://nno.ppjwa.cn

[R45] 批量删除
来源：http://npq.c1oappe.top

find . -name "*.tmp" -delete
来源：http://gyt.jiagoushi.top

[R46] 递归替换文件内容
来源：http://bcq.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nan.nanxuanxn.top

[R47] sed 单行替换
来源：http://ceg.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://jnq.yonumen.top

[R48] awk 取指定列
来源：http://sys.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://kda.sweek.top

[R49] awk 带条件
来源：http://dyo.sxryk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qub.redwolf501.top

[R50] awk 求和
来源：http://pbw.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://jtw.iojbl.cn

[R51] 排序去重取前几
来源：http://nck.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qik.nwbrower.top

[R52] 统计行数
来源：http://seh.ydzc1.top

wc -l a.txt
来源：http://poi.yj20258888.top

[R53] 查看文件头与实时尾
来源：http://vse.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mxy.xuanzx.com

[R54] 比较两个文件
来源：http://agp.gotoacloud.top

diff a.txt b.txt
来源：http://vfh.yfazqb.com

[R55] 压缩与解压
来源：http://kem.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tbm.zhixingplan.top

[R56] 远程拷贝
来源：http://krc.hnxiangtu.top

scp file user@host:/path/
来源：http://ssi.shuidangran.top

[R57] 远程执行命令
来源：http://pmi.hywenlv.cn

ssh user@host 'uptime'
来源：http://akj.ydjk.org.cn

[R58] 下载文件
来源：http://ftr.shuidangran.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cdq.yanxiufei.cn

[R59] 发 POST JSON
来源：http://xiu.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://huh.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://jqj.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nzy.redwolf501.top

[R61] 磁盘占用
来源：http://tbx.gzhubu.top

df -h;  du -sh *
来源：http://dwx.bjfxy.top

[R62] 找最占空间的文件
来源：http://zqp.tianlin.xyz

du -ah . | sort -rh | head -10
来源：http://wuy.guowangkeji.top

[R63] 内存与进程
来源：http://swl.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://tbm.jlsjyb.cn

[R64] 结束进程
来源：http://sww.hongshengwenyu.top

kill -9 $(pgrep -f app.py)
来源：http://giy.cheryme.top

[R65] 查看端口占用
来源：http://alk.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lir.birdmap.top

[R66] 定时任务
来源：http://lol.gaohongyu789.top

crontab -e;  crontab -l
来源：http://qza.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://kux.jqgufenzy.top

openssl rand -hex 16
来源：http://soz.cashguo.top

[R68] 计算文件校验值
来源：http://byr.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wes.zhengqikj.top

[R69] 生成随机密码
来源：http://acv.meibo888.top

head -c 16 /dev/urandom | base64
来源：http://cgq.nwbrower.top

[R70] 时间戳与互转
来源：http://qzw.aizwys.cn

date +%s;  date -d @1700000000
来源：http://wqb.cashguo.top

[R71] 日期格式化
来源：http://poz.wangshuangyany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://non.yj202588.top

[R72] 等待端口就绪
来源：http://oac.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hwy.gogol.net.cn

[R73] 分割大日志
来源：http://udp.dianchejie.cn

split -l 1000 big.log part_
来源：http://ooa.jianghu66.top

[R74] 批量重命名
来源：http://tfe.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lku.sweek.top

[R75] 导出环境变量
来源：http://qxp.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://gkz.svipenyu.cn

[R76] 使用临时文件
来源：http://dwo.dashuyun.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vwt.nanxinkj.top

[R77] 读取用户输入
来源：http://ewu.tian-w.cn

read -rp "请输入: " ans
来源：http://kgj.uphjek.com

[R78] 交互式菜单
来源：http://wya.gaohongyu789.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vkg.kuanghao11.cn

[R79] 解析命令行选项
来源：http://kqg.cqqwz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tsr.yongpay.top

[R80] 查看脚本执行耗时
来源：http://kjp.9152youxi.cn

time ./run.sh
来源：http://ynn.hcnkem.com

================================================================================
来源：http://swy.gaohongyu789.top

S. C / C++ 专题
来源：http://ipt.wangdashe.top

================================================================================
来源：http://tvi.fzhhl.top

[S01] C：Hello World
来源：http://daj.9152youxi.cn

#include <stdio.h>
来源：http://rtj.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://izk.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://zio.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://jhs.yuxming.cn

[S03] C：读入整数
来源：http://mpg.yj202588.top

int x; scanf("%d", &x);
来源：http://sxw.hfpthk.cn

[S04] C：字符串复制
来源：http://smq.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gab.sxryk.cn

[S05] C：字符串长度
来源：http://rdu.yvedp.cn

strlen(s)
来源：http://vfk.guowangkeji.top

[S06] C：字符串比较
来源：http://fhv.sysykeji.top

strcmp(a, b) == 0
来源：http://kzn.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://lsq.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rjl.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://fof.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qix.hcnkem.com

[S09] C：结构体定义与初始化
来源：http://rew.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lmo.jqgufenzy.top

[S10] C：指针与解引用
来源：http://tzw.jinqigufen.top

int *p = &a;  *p = 5;
来源：http://jrq.zhijiandao.cn

[S11] C：逐行读文件
来源：http://yer.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://hyi.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ehd.fktsv.cn

fclose(f);
来源：http://vsf.gaohongyu789.top

[S12] C：写文件
来源：http://bus.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bbl.yuxming.cn

[S13] C：宏定义
来源：http://lpl.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ama.ehwqpu.com

[S14] C：枚举
来源：http://pxp.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://pil.hammf.cn

[S15] C：类型转换
来源：http://pxw.tian-w.cn

(double) a / b
来源：http://jgo.snrcjt.cn

[S16] C：位操作置位
来源：http://cyk.shzxlz.cn

x |= (1 << 3);
来源：http://hmw.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://mzb.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://grq.vqdsnc.cn

[S18] C：命令行参数
来源：http://meb.sxryk.cn

int main(int argc, char **argv)
来源：http://fvr.mhx1999.top

[S19] C：快速排序
来源：http://khx.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://xhs.52xcode.cn

[S20] C：二分查找
来源：http://vpu.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ymq.yuxming.cn

[S21] C：字符类别判断
来源：http://wnn.guowangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://suf.316326.xyz

[S22] C：字符串转数字
来源：http://vzq.fktsv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vdf.jinghuilouyu.cn

[S23] C：随机数
来源：http://wct.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://flu.shuidangran.top

[S24] C：获取本地时间
来源：http://zob.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gog.yfazqb.com

[S25] C：内存拷贝
来源：http://qwb.jiagoushi.top

memcpy(dst, src, n);
来源：http://ugi.jinqigfzy.top

[S26] C：内存清零
来源：http://dby.nanxinkj.top

memset(a, 0, sizeof a);
来源：http://skr.fanxiaobao.xyz

[S27] C：定义常量
来源：http://kfy.shangyingyoupin.top

const double PI = 3.14159;
来源：http://rrz.zdqjudy.top

[S28] C：静态变量
来源：http://bth.yvedp.cn

static int counter = 0;
来源：http://ueo.cheryme.top

[S29] C：变参函数
来源：http://mar.yanxiufei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jtz.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://ebk.sysykeji.top

#ifndef X_H
来源：http://ztn.jqgufenzy.top

#define X_H
来源：http://krg.yangfankeji.com

#endif
来源：http://qal.gotoacloud.top

[S31] C++：Hello World
来源：http://wrz.hfpthk.cn

#include <iostream>
来源：http://juf.cdnleiting.top

int main() { std::cout << "Hello\n"; }
来源：http://qib.nwbrower.top

[S32] C++：字符串
来源：http://lei.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://anq.jyoumei.cn

[S33] C++：vector 增删
来源：http://sbl.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fuz.hysaishi.cn

[S34] C++：遍历 vector
来源：http://pfz.yangfankeji.com

for (auto &x : v) { std::cout << x; }
来源：http://uxn.jlsjyb.cn

[S35] C++：map
来源：http://alp.tanke756.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kzc.gzhubu.top

[S36] C++：unordered_map
来源：http://sgg.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fve.ybcxt.top

[S37] C++：set
来源：http://sjr.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://css.9152youxi.cn

[S38] C++：排序
来源：http://heo.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://iok.chenlongwang.top

[S39] C++：自定义比较器排序
来源：http://yvt.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vmo.vqdsnc.cn

[S40] C++：查找元素
来源：http://oed.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nbn.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://qwm.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://alx.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://ius.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://map.jiagoushi.top

[S43] C++：智能指针
来源：http://qng.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://vsw.xinyue.icu

[S44] C++：引用传参
来源：http://tnf.svipenyu.cn

void inc(int &x) { ++x; }
来源：http://zcm.yueranfly.top

[S45] C++：lambda
来源：http://qsh.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://qie.jlsjyb.cn

[S46] C++：函数模板
来源：http://hec.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qys.aizwys.cn

[S47] C++：结构化绑定遍历
来源：http://afw.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sfu.aizwys.cn

[S48] C++：逐行读文件
来源：http://tdz.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://qky.tanke756.top

while (std::getline(in, line)) { }
来源：http://yrr.gzhubu.top

[S49] C++：写文件
来源：http://vtr.xuetiantiany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hsq.zhoulong.xyz

[S50] C++：格式化数字
来源：http://ios.fktsv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oyi.daxiang520.top

[S51] C++：显式类型转换
来源：http://uyw.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://ukw.cashguo.top

[S52] C++：const 与 noexcept
来源：http://oih.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://odl.sxryk.cn

[S53] C++：移动语义
来源：http://lna.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://fzb.svipenyu.cn

[S54] C++：异常处理
来源：http://xcr.hnxiangtu.top


<!-- 参考信息 -->