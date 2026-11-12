代发 wailian999

[Q84] 去除首尾空格
来源：http://zqn.dashuyun.cn

SELECT TRIM(name) FROM users;
来源：http://ufe.fengsongda.top

[Q85] 数值取整
来源：http://mxl.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kcw.yuxming.cn

[Q86] 读取 JSON 字段
来源：http://ltb.aibaodan.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wqj.iojbl.cn

[Q87] JSON 字段做条件
来源：http://lkp.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fhz.xuanzx.com

[Q88] 行转列（条件聚合）
来源：http://nvw.kuanghao11.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rnu.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hcy.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://kxc.xylfe.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kzr.uphjek.com

[Q90] 生成序号列
来源：http://uyc.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://anv.tarul.cn

================================================================================
来源：http://tfm.andypj.xyz

R. Bash 专题
来源：http://hpp.xuetiantiany.cn

================================================================================
来源：http://bos.0kj1m.cn

[R01] shebang 与严格模式
来源：http://uwb.tarul.cn

#!/usr/bin/env bash
来源：http://cvg.hongshengwenyu.top

set -euo pipefail
来源：http://kze.dashuyun.cn

[R02] 变量赋值与使用
来源：http://fbo.52xcode.cn

name="Tom"; echo "$name"
来源：http://chs.yuxming.cn

[R03] 只读变量
来源：http://mvw.xuanzx.com

readonly PI=3.14
来源：http://pwu.daxiang520.top

[R04] 位置参数
来源：http://ksv.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xtb.cucudq.cn

[R05] 参数默认值
来源：http://iwu.fengsongda.top

name="${1:-default}"
来源：http://swc.gogol.net.cn

[R06] 判断命令是否存在
来源：http://lbs.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mpk.meibo888.top

[R07] if 判断文件
来源：http://qbq.fzhhl.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ner.yongpay.top

[R08] 数值比较
来源：http://cwq.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wbk.9152youxi.cn

[R09] 字符串比较
来源：http://smi.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ntb.svipenyu.cn

[R10] 正则匹配
来源：http://lcn.jiagoushi.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ord.pengpengdd.cyou

[R11] case 多分支
来源：http://mfu.ctjpmb.com

case "$1" in
来源：http://zru.zycfv.cn

start) echo "启动" ;;
来源：http://und.pengpengdd.cyou

stop)  echo "停止" ;;
来源：http://vin.tian-w.cn

*)     echo "未知命令" ;;
来源：http://wfc.shanyushiyangtech.top

esac
来源：http://esl.jiagoushi.top

[R12] for 遍历文件
来源：http://qhc.bbcook.cn

for f in *.txt; do echo "$f"; done
来源：http://bvd.yj202588.top

[R13] for 计数循环
来源：http://rwy.meibo888.top

for i in {1..10}; do echo "$i"; done
来源：http://gun.jiagoushi.top

[R14] C 风格 for
来源：http://bzv.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jdj.wangdashe.top

[R15] while 逐行读文件
来源：http://ryb.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hdz.iojbl.cn

[R16] until 等待条件
来源：http://lck.gaohongyu789.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rmz.snrcjt.cn

[R17] 数组定义与取值
来源：http://mqz.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://tsj.jinqigfzy.top

[R18] 遍历数组
来源：http://mnv.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ggd.hesvh.cn

[R19] 数组长度
来源：http://vdq.guowangkeji.top

echo "${#arr[@]}"
来源：http://hta.shzxlz.cn

[R20] 关联数组（字典）
来源：http://dnl.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bia.daria6918.cn

[R21] 字符串长度
来源：http://zcr.epnwcf.com

echo "${#s}"
来源：http://chz.tian-w.cn

[R22] 截取子串
来源：http://vvn.fehbvm.com

echo "${s:0:5}"
来源：http://xnw.zhengqikj.top

[R23] 字符串替换
来源：http://kgm.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vmc.snrcjt.cn

[R24] 大小写转换
来源：http://wsp.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://nmb.bbcook.cn

[R25] 去后缀 / 去前缀
来源：http://uzy.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jnr.snrcjt.cn

[R26] 命令替换
来源：http://erl.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://chs.pycfn.com

[R27] 算术展开
来源：http://imo.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://kql.fktsv.cn

[R28] 浮点运算
来源：http://etk.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://jwg.dianchejie.cn

[R29] 定义函数
来源：http://yhx.sysykeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://idc.fzhhl.top

[R30] 函数返回状态码
来源：http://dzg.shangyingyoupin.top

f() { return 0; }; f || echo "失败了"
来源：http://bwf.havefunace.top

[R31] 局部变量
来源：http://kkj.hnqzz.top

f() { local x=1; echo "$x"; }
来源：http://eql.yonumen.top

[R32] 参数个数校验
来源：http://gfe.xuetiantiany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tgy.vqdsnc.cn

[R33] 捕获错误并提示行号
来源：http://wjr.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rnz.zhongyouzk.top

[R34] 退出时清理
来源：http://qpq.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://she.aibaodan.cn

[R35] 后台执行并等待
来源：http://ukl.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rzf.havefunace.top

[R36] 并发执行多个任务
来源：http://iaz.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ljr.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://jeb.fengsongda.top

files=$(ls -1)
来源：http://jhp.9152youxi.cn

[R38] 管道串联
来源：http://kff.tarul.cn

cat a.txt | grep -i error | wc -l
来源：http://zjy.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://fve.shuidangran.top

cmd > out.log 2>&1
来源：http://anx.hfpthk.cn

[R40] 追加写日志
来源：http://unm.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://exn.hesvh.cn

[R41] 丢弃输出
来源：http://scj.hnqzz.top

cmd >/dev/null 2>&1
来源：http://qmm.nanxinkj.top

[R42] 输入重定向
来源：http://sbv.redwolf501.top

wc -l < a.txt
来源：http://vlf.hcnkem.com

[R43] 按名字查找文件
来源：http://fgd.vqdsnc.cn

find . -name "*.log" -type f
来源：http://kcg.shuidangran.top

[R44] 按修改时间查找
来源：http://dvp.fktsv.cn

find . -mtime -7 -type f
来源：http://rgp.gzhubu.top

[R45] 批量删除
来源：http://erv.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://awh.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://hpu.daria6918.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ofq.zhengqikj.top

[R47] sed 单行替换
来源：http://ghz.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wbo.jiagoushi.top

[R48] awk 取指定列
来源：http://nha.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://gyq.yangfankeji.com

[R49] awk 带条件
来源：http://ahx.zdbjq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tfq.chenzaomai.com

[R50] awk 求和
来源：http://ttw.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hhz.hesvh.cn

[R51] 排序去重取前几
来源：http://evi.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yfr.yj20258888.top

[R52] 统计行数
来源：http://szo.daxiang520.top

wc -l a.txt
来源：http://yjj.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://hok.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uhb.yvedp.cn

[R54] 比较两个文件
来源：http://nba.hcnkem.com

diff a.txt b.txt
来源：http://cik.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://lxd.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rjs.yonumen.top

[R56] 远程拷贝
来源：http://oqz.smart0.xyz

scp file user@host:/path/
来源：http://fod.ctjpmb.com

[R57] 远程执行命令
来源：http://prj.mhx1999.top

ssh user@host 'uptime'
来源：http://pie.redwolf501.top

[R58] 下载文件
来源：http://gif.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jzl.yangfankeji.com

[R59] 发 POST JSON
来源：http://gnt.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xdm.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://fkw.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kxo.jqgfzy.top

[R61] 磁盘占用
来源：http://wuq.hnqzz.top

df -h;  du -sh *
来源：http://dkk.xziqi.cn

[R62] 找最占空间的文件
来源：http://jsc.havefunace.top

du -ah . | sort -rh | head -10
来源：http://obu.svipenyu.cn

[R63] 内存与进程
来源：http://tux.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://ltg.gaohongyu789.top

[R64] 结束进程
来源：http://diz.shuidangran.top

kill -9 $(pgrep -f app.py)
来源：http://vko.nanxinkj.top

[R65] 查看端口占用
来源：http://fos.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://khw.tianlin.xyz

[R66] 定时任务
来源：http://ybr.jyoumei.cn

crontab -e;  crontab -l
来源：http://ssu.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://meg.yongpay.top

openssl rand -hex 16
来源：http://jhx.daxiang520.top

[R68] 计算文件校验值
来源：http://pne.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://nul.fehbvm.com

[R69] 生成随机密码
来源：http://cdh.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://gdq.xinyue.icu

[R70] 时间戳与互转
来源：http://ste.tian-w.cn

date +%s;  date -d @1700000000
来源：http://yyb.gaohongyu789.top

[R71] 日期格式化
来源：http://hig.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rbx.kuanghao11.cn

[R72] 等待端口就绪
来源：http://jga.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wph.yfazqb.com

[R73] 分割大日志
来源：http://zhr.cheryme.top

split -l 1000 big.log part_
来源：http://ymx.andypj.xyz

[R74] 批量重命名
来源：http://twe.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gws.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://nfe.zhiwuduotai.top

export PATH="$HOME/bin:$PATH"
来源：http://zdm.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://rsv.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cem.wangshuangyany.cn

[R77] 读取用户输入
来源：http://omz.redwolf501.top

read -rp "请输入: " ans
来源：http://kcf.zhoulong.xyz

[R78] 交互式菜单
来源：http://nol.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yhy.meibo888.top

[R79] 解析命令行选项
来源：http://hpo.ivvv.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hho.havefunace.top

[R80] 查看脚本执行耗时
来源：http://wkl.iojbl.cn

time ./run.sh
来源：http://tib.zhijiandao.cn

================================================================================
来源：http://tpo.smart0.xyz

S. C / C++ 专题
来源：http://onr.epnwcf.com

================================================================================
来源：http://rdq.dashuyun.cn

[S01] C：Hello World
来源：http://spi.zhaomingkeji.xyz

#include <stdio.h>
来源：http://mtz.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://ahs.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://opy.jinqigfzy.top

int a = 10; printf("%d\n", a);
来源：http://tzw.snrcjt.cn

[S03] C：读入整数
来源：http://mkl.smart0.xyz

int x; scanf("%d", &x);
来源：http://zcy.cdnleiting.top

[S04] C：字符串复制
来源：http://ovx.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://aei.sxryk.cn

[S05] C：字符串长度
来源：http://edg.pycfn.com

strlen(s)
来源：http://thy.hfpthk.cn

[S06] C：字符串比较
来源：http://uns.hfpthk.cn

strcmp(a, b) == 0
来源：http://aon.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://gjz.yj202588.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://puh.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://ocb.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oqh.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://ery.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vzo.xingfuxueyuan.xyz

[S10] C：指针与解引用
来源：http://rbx.fehbvm.com

int *p = &a;  *p = 5;
来源：http://gcy.tian-w.cn

[S11] C：逐行读文件
来源：http://ppt.jinqigfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://siz.sufxvd.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mcr.sweek.top

fclose(f);
来源：http://evo.zhaomingkeji.xyz

[S12] C：写文件
来源：http://flz.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xvf.tianlin.xyz

[S13] C：宏定义
来源：http://pka.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://geu.ivvv.top

[S14] C：枚举
来源：http://ahm.tian-w.cn

enum Color { RED, GREEN, BLUE };
来源：http://czz.ppjwa.cn

[S15] C：类型转换
来源：http://xew.vehdjk.com

(double) a / b
来源：http://kth.nanxuanxn.top

[S16] C：位操作置位
来源：http://jqd.jinghuilouyu.cn

x |= (1 << 3);
来源：http://jan.nwbrower.top

[S17] C：安全拼接字符串
来源：http://ktm.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ohs.zhijiandao.cn

[S18] C：命令行参数
来源：http://iao.zhengqikj.top

int main(int argc, char **argv)
来源：http://dsb.haohaochexian.top

[S19] C：快速排序
来源：http://vkb.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://drm.jianghu66.top

[S20] C：二分查找
来源：http://hlg.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gdd.aizwys.cn

[S21] C：字符类别判断
来源：http://cfm.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xti.kuanghao11.cn

[S22] C：字符串转数字
来源：http://mqi.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tfy.sxryk.cn

[S23] C：随机数
来源：http://ins.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://edm.yj20258888.top

[S24] C：获取本地时间
来源：http://uah.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ird.pycfn.com

[S25] C：内存拷贝
来源：http://def.hcnkem.com

memcpy(dst, src, n);
来源：http://pea.zhiwuduotai.top

[S26] C：内存清零
来源：http://nvw.yfazqb.com

memset(a, 0, sizeof a);
来源：http://ezv.tarul.cn

[S27] C：定义常量
来源：http://nox.dashuyun.cn

const double PI = 3.14159;
来源：http://bfw.gogol.net.cn

[S28] C：静态变量
来源：http://tjo.0kj1m.cn

static int counter = 0;
来源：http://iwf.yongpay.top

[S29] C：变参函数
来源：http://rts.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jtp.zhiwuduotai.top

[S30] C：头文件保护
来源：http://mep.nanxuanxn.top

#ifndef X_H
来源：http://mla.epnwcf.com

#define X_H
来源：http://ylj.hongshengwenyu.top

#endif
来源：http://zjj.hongshengwenyu.top

[S31] C++：Hello World
来源：http://vgn.dashuyun.cn

#include <iostream>
来源：http://xba.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://red.zhiwuduotai.top

[S32] C++：字符串
来源：http://bvb.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://llx.yongpay.top

[S33] C++：vector 增删
来源：http://bvn.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iup.tanke756.top

[S34] C++：遍历 vector
来源：http://rce.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://mio.cashguo.top

[S35] C++：map
来源：http://mhg.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pyf.xinyue.icu

[S36] C++：unordered_map
来源：http://vki.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://phc.cheryme.top

[S37] C++：set
来源：http://knw.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ypj.shanyushiyangkeji.top

[S38] C++：排序
来源：http://rrx.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://kvq.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://qhg.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wnd.zdqjudy.top

[S40] C++：查找元素
来源：http://mgl.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jxl.yuanzhike.top

[S41] C++：类与构造函数
来源：http://zfi.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cgi.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://xxu.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://fks.yonumen.top

[S43] C++：智能指针
来源：http://oeb.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://cyh.hcnkem.com

[S44] C++：引用传参
来源：http://pjv.zhoulong.xyz

void inc(int &x) { ++x; }
来源：http://ptu.tian-w.cn

[S45] C++：lambda
来源：http://vnc.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://zgf.shangyingyoupin.top

[S46] C++：函数模板
来源：http://dkd.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tqq.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://bsc.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aql.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://tso.nanxinkj.top

std::ifstream in("a.txt");  std::string line;
来源：http://fge.aizwys.cn

while (std::getline(in, line)) { }
来源：http://voi.chenzaomai.com

[S49] C++：写文件
来源：http://vkl.xziqi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rcz.fktsv.cn

[S50] C++：格式化数字
来源：http://xrk.vqdsnc.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kbn.yj202588.top

[S51] C++：显式类型转换
来源：http://dns.bjfxy.top

static_cast<double>(a) / b
来源：http://gaj.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://rsh.yuanzhike.top

int size() const noexcept { return n_; }
来源：http://wqn.jqgfzy.top

[S53] C++：移动语义
来源：http://hdo.havefunace.top

std::vector<int> w = std::move(v);
来源：http://ebq.xuanzx.com

[S54] C++：异常处理
来源：http://kcp.wangshuangyany.cn


<!-- 参考信息 -->