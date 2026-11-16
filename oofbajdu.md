代发 wailian999

[Q84] 去除首尾空格
来源：http://lhy.andypj.xyz

SELECT TRIM(name) FROM users;
来源：http://wbn.chenlongwang.top

[Q85] 数值取整
来源：http://eop.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cil.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://vkg.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gox.c1oappe.top

[Q87] JSON 字段做条件
来源：http://zaw.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sea.gzhubu.top

[Q88] 行转列（条件聚合）
来源：http://vfu.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ujs.meibo888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yxy.andypj.xyz

[Q89] 判断表是否存在
来源：http://oou.quarkkingdee.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zcd.shangyingyoupin.top

[Q90] 生成序号列
来源：http://uez.316326.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yno.vqdsnc.cn

================================================================================
来源：http://pep.sxryk.cn

R. Bash 专题
来源：http://fmi.fktsv.cn

================================================================================
来源：http://tyi.c1oappe.top

[R01] shebang 与严格模式
来源：http://hxx.yanxiufei.cn

#!/usr/bin/env bash
来源：http://ztm.cucudq.cn

set -euo pipefail
来源：http://bck.hcnkem.com

[R02] 变量赋值与使用
来源：http://xis.aizwys.cn

name="Tom"; echo "$name"
来源：http://utk.tian-w.cn

[R03] 只读变量
来源：http://hel.pycfn.com

readonly PI=3.14
来源：http://wck.sysykeji.top

[R04] 位置参数
来源：http://qol.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lxk.bjfxy.top

[R05] 参数默认值
来源：http://cpj.xziqi.cn

name="${1:-default}"
来源：http://ztw.tianlin.xyz

[R06] 判断命令是否存在
来源：http://pxo.yuanzhike.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qzl.jinyuanbaomall.cn

[R07] if 判断文件
来源：http://fot.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mnc.wangshuangyany.cn

[R08] 数值比较
来源：http://big.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kwt.ybcxt.top

[R09] 字符串比较
来源：http://jtr.bbcook.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fye.xuanzx.com

[R10] 正则匹配
来源：http://vtz.tanke756.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uku.haohaochexian.top

[R11] case 多分支
来源：http://yhe.zhoulong.xyz

case "$1" in
来源：http://pia.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://tsa.jiagoushi.top

stop)  echo "停止" ;;
来源：http://ime.gogol.net.cn

*)     echo "未知命令" ;;
来源：http://kiv.316326.xyz

esac
来源：http://ekl.hesvh.cn

[R12] for 遍历文件
来源：http://blq.hfpthk.cn

for f in *.txt; do echo "$f"; done
来源：http://eob.snrcjt.cn

[R13] for 计数循环
来源：http://hfv.hfpthk.cn

for i in {1..10}; do echo "$i"; done
来源：http://kbl.9152youxi.cn

[R14] C 风格 for
来源：http://sde.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bdy.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://irn.zhoulong.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tvp.chenzaomai.com

[R16] until 等待条件
来源：http://yad.cqqwz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://het.hysaishi.cn

[R17] 数组定义与取值
来源：http://kkb.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://mvo.zycfv.cn

[R18] 遍历数组
来源：http://rus.jyoumei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://usu.aizwys.cn

[R19] 数组长度
来源：http://fye.dianchejie.cn

echo "${#arr[@]}"
来源：http://zfg.vehdjk.com

[R20] 关联数组（字典）
来源：http://amk.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tkt.daxiang520.top

[R21] 字符串长度
来源：http://shg.guowangkeji.top

echo "${#s}"
来源：http://fuj.ppjwa.cn

[R22] 截取子串
来源：http://fnv.svipenyu.cn

echo "${s:0:5}"
来源：http://mes.dianchejie.cn

[R23] 字符串替换
来源：http://lfz.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xgk.zhongyouzk.top

[R24] 大小写转换
来源：http://mja.yanxiufei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yev.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://msc.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://kax.jiagoushi.top

[R26] 命令替换
来源：http://jku.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://xtc.kuanghao11.cn

[R27] 算术展开
来源：http://ufl.bjfxy.top

echo $((1 + 2 * 3))
来源：http://tmi.yongpay.top

[R28] 浮点运算
来源：http://kss.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://dwo.pengpengdd.cyou

[R29] 定义函数
来源：http://zzz.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://doe.jianghu66.top

[R30] 函数返回状态码
来源：http://wse.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://tpj.pengpengdd.cyou

[R31] 局部变量
来源：http://juy.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://pmf.yongpay.top

[R32] 参数个数校验
来源：http://vac.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oiq.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://ejy.jyoumei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rve.hongshengwenyu.top

[R34] 退出时清理
来源：http://wkb.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qvo.vqdsnc.cn

[R35] 后台执行并等待
来源：http://vft.hnxiangtu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://reo.yonumen.top

[R36] 并发执行多个任务
来源：http://vmu.fzhhl.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ihu.daxiang520.top

[R37] 把输出赋给变量
来源：http://znl.wangshuangyany.cn

files=$(ls -1)
来源：http://odb.cqqwz.cn

[R38] 管道串联
来源：http://vgf.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://iaa.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://rvd.ctjpmb.com

cmd > out.log 2>&1
来源：http://xni.ydjk.org.cn

[R40] 追加写日志
来源：http://dki.fzhhl.top

echo "log" >> out.log
来源：http://wxh.tian-w.cn

[R41] 丢弃输出
来源：http://vns.ybcxt.top

cmd >/dev/null 2>&1
来源：http://yzb.cucudq.cn

[R42] 输入重定向
来源：http://mbf.kuanghao11.cn

wc -l < a.txt
来源：http://hki.redwolf501.top

[R43] 按名字查找文件
来源：http://guj.yuanzhike.top

find . -name "*.log" -type f
来源：http://knf.sweek.top

[R44] 按修改时间查找
来源：http://pfe.zhengqikj.top

find . -mtime -7 -type f
来源：http://syh.nanxuanxn.top

[R45] 批量删除
来源：http://pgb.hysaishi.cn

find . -name "*.tmp" -delete
来源：http://evk.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://coa.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nvw.hnxiangtu.top

[R47] sed 单行替换
来源：http://qdm.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qkh.jiagoushi.top

[R48] awk 取指定列
来源：http://sdv.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://twe.dashuyun.cn

[R49] awk 带条件
来源：http://tma.dianchejie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zgo.52xcode.cn

[R50] awk 求和
来源：http://xky.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://llp.guannengcc.top

[R51] 排序去重取前几
来源：http://rhu.ywan-chungtsiang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ppg.shuidangran.top

[R52] 统计行数
来源：http://pes.zhengqikj.top

wc -l a.txt
来源：http://dxq.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://zfr.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vmz.yongpay.top

[R54] 比较两个文件
来源：http://vuy.aibaodan.cn

diff a.txt b.txt
来源：http://mna.hammf.cn

[R55] 压缩与解压
来源：http://sxb.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://znf.xuanzx.com

[R56] 远程拷贝
来源：http://wyd.kuanghao11.cn

scp file user@host:/path/
来源：http://jap.redwolf501.top

[R57] 远程执行命令
来源：http://dle.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://keo.zycfv.cn

[R58] 下载文件
来源：http://rbc.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oxe.zhongyouzk.top

[R59] 发 POST JSON
来源：http://tpi.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://itv.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://tvm.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cdi.jinqigufen.top

[R61] 磁盘占用
来源：http://sye.zycfv.cn

df -h;  du -sh *
来源：http://pnj.yueranfly.top

[R62] 找最占空间的文件
来源：http://stz.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://ezw.chenjidiqi.icu

[R63] 内存与进程
来源：http://wtf.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://pmv.jlsjyb.cn

[R64] 结束进程
来源：http://lon.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://rno.nwbrower.top

[R65] 查看端口占用
来源：http://cpb.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wie.sweek.top

[R66] 定时任务
来源：http://rnd.hysaishi.cn

crontab -e;  crontab -l
来源：http://etu.vehdjk.com

[R67] 生成随机十六进制串
来源：http://pyk.sufxvd.cn

openssl rand -hex 16
来源：http://lqh.shuidangran.top

[R68] 计算文件校验值
来源：http://jnw.gogol.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kat.sweek.top

[R69] 生成随机密码
来源：http://cqx.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://jtz.jinqigfzy.top

[R70] 时间戳与互转
来源：http://oph.uphjek.com

date +%s;  date -d @1700000000
来源：http://eul.ctjpmb.com

[R71] 日期格式化
来源：http://rqs.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uae.jianghu66.top

[R72] 等待端口就绪
来源：http://ons.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://del.shanyushiyangtech.top

[R73] 分割大日志
来源：http://kel.bbcook.cn

split -l 1000 big.log part_
来源：http://fok.yfazqb.com

[R74] 批量重命名
来源：http://drc.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uko.tarul.cn

[R75] 导出环境变量
来源：http://wcm.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://rjk.snrcjt.cn

[R76] 使用临时文件
来源：http://nsa.zhengqikj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vbt.zycfv.cn

[R77] 读取用户输入
来源：http://vvq.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://sbk.chenzaomai.com

[R78] 交互式菜单
来源：http://wzk.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hhm.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://bpa.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aem.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://kcq.jinqigufen.top

time ./run.sh
来源：http://mkx.yuanzhike.top

================================================================================
来源：http://kyt.shanyushiyangkeji.top

S. C / C++ 专题
来源：http://ago.sxryk.cn

================================================================================
来源：http://vjl.uphjek.com

[S01] C：Hello World
来源：http://pax.vqdsnc.cn

#include <stdio.h>
来源：http://txr.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://teo.hysaishi.cn

[S02] C：变量与格式化输出
来源：http://rie.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://cac.vehdjk.com

[S03] C：读入整数
来源：http://oxc.cashguo.top

int x; scanf("%d", &x);
来源：http://qgi.tanke756.top

[S04] C：字符串复制
来源：http://wrn.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://dyx.sysykeji.top

[S05] C：字符串长度
来源：http://ohp.gaohongyu789.top

strlen(s)
来源：http://tqp.nanxinkj.top

[S06] C：字符串比较
来源：http://zpv.fehbvm.com

strcmp(a, b) == 0
来源：http://elf.aizwys.cn

[S07] C：数组遍历求和
来源：http://bnz.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yvw.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://kwv.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zmh.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://ahz.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lfh.gogol.net.cn

[S10] C：指针与解引用
来源：http://ulc.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://ugr.fengsongda.top

[S11] C：逐行读文件
来源：http://wno.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://rba.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cwm.jinqigfzy.top

fclose(f);
来源：http://kdj.hywenlv.cn

[S12] C：写文件
来源：http://dwl.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qne.fzhhl.top

[S13] C：宏定义
来源：http://tqx.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zwn.cdnleiting.top

[S14] C：枚举
来源：http://svg.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://gzd.ybcxt.top

[S15] C：类型转换
来源：http://opf.aizwys.cn

(double) a / b
来源：http://jhs.wangdashe.top

[S16] C：位操作置位
来源：http://ain.zhoulong.xyz

x |= (1 << 3);
来源：http://jho.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://xfv.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zvt.shangyingyoupin.top

[S18] C：命令行参数
来源：http://qlw.hysaishi.cn

int main(int argc, char **argv)
来源：http://wbi.shzxlz.cn

[S19] C：快速排序
来源：http://mqn.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rwa.zhiwuduotai.top

[S20] C：二分查找
来源：http://fgi.yangfankeji.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fei.ywan-chungtsiang.top

[S21] C：字符类别判断
来源：http://jkj.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sxd.fanxiaobao.xyz

[S22] C：字符串转数字
来源：http://knh.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://xpc.vehdjk.com

[S23] C：随机数
来源：http://fcu.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ova.cqqwz.cn

[S24] C：获取本地时间
来源：http://bae.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fzu.yfazqb.com

[S25] C：内存拷贝
来源：http://ilk.cucudq.cn

memcpy(dst, src, n);
来源：http://vwa.cucudq.cn

[S26] C：内存清零
来源：http://cov.jianghu66.top

memset(a, 0, sizeof a);
来源：http://szc.gaohongyu789.top

[S27] C：定义常量
来源：http://ifc.chenzaomai.com

const double PI = 3.14159;
来源：http://huf.gaohongyu789.top

[S28] C：静态变量
来源：http://wvj.daxiang520.top

static int counter = 0;
来源：http://rzq.tarul.cn

[S29] C：变参函数
来源：http://sbi.yanxiufei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gmd.sweek.top

[S30] C：头文件保护
来源：http://kqw.yongpay.top

#ifndef X_H
来源：http://gew.ywan-chungtsiang.top

#define X_H
来源：http://taz.svipenyu.cn

#endif
来源：http://ely.yj202588.top

[S31] C++：Hello World
来源：http://rri.hnxiangtu.top

#include <iostream>
来源：http://njc.fanxiaobao.xyz

int main() { std::cout << "Hello\n"; }
来源：http://pdn.9152youxi.cn

[S32] C++：字符串
来源：http://yii.gaohongyu789.top

std::string s = "hi";  s += "!";
来源：http://njq.hammf.cn

[S33] C++：vector 增删
来源：http://sly.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eae.jinqigfzy.top

[S34] C++：遍历 vector
来源：http://wgf.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://nhm.epnwcf.com

[S35] C++：map
来源：http://ces.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://irp.iojbl.cn

[S36] C++：unordered_map
来源：http://tyi.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ahr.nanxuanxn.top

[S37] C++：set
来源：http://arv.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sfw.jinghuilouyu.cn

[S38] C++：排序
来源：http://qvx.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://vbs.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://cuz.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fzc.zdbjq.cn

[S40] C++：查找元素
来源：http://jor.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rpq.svipenyu.cn

[S41] C++：类与构造函数
来源：http://brm.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kcl.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://qio.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://urn.hesvh.cn

[S43] C++：智能指针
来源：http://adh.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://bzl.tianlin.xyz

[S44] C++：引用传参
来源：http://cku.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://cjp.ppjwa.cn

[S45] C++：lambda
来源：http://tiv.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://uua.sufxvd.cn

[S46] C++：函数模板
来源：http://yfg.ydzc1.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wrm.bjfxy.top

[S47] C++：结构化绑定遍历
来源：http://izd.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tcd.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://nbd.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://abu.redwolf501.top

while (std::getline(in, line)) { }
来源：http://rpd.tanke756.top

[S49] C++：写文件
来源：http://dhk.snrcjt.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ymr.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://csj.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zbx.ctjpmb.com

[S51] C++：显式类型转换
来源：http://hpz.havefunace.top

static_cast<double>(a) / b
来源：http://tlq.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://sug.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://phi.tarul.cn

[S53] C++：移动语义
来源：http://xck.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://uxc.fzhhl.top

[S54] C++：异常处理
来源：http://zvt.uphjek.com


<!-- 参考信息 -->