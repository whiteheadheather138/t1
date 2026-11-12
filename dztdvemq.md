代发 wailian999

[Q82] 字符长度与字节长度
来源：http://une.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rmk.fktsv.cn

[Q83] 大小写转换
来源：http://zbj.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mks.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://amz.cashguo.top

SELECT TRIM(name) FROM users;
来源：http://zej.tian-w.cn

[Q85] 数值取整
来源：http://cbw.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://umw.jinqigufen.top

[Q86] 读取 JSON 字段
来源：http://whe.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uvq.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://yhz.cashguo.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fqx.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://lcw.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hie.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hqz.hywenlv.cn

[Q89] 判断表是否存在
来源：http://rub.vehdjk.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zsa.jianghu66.top

[Q90] 生成序号列
来源：http://zur.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://itl.0kj1m.cn

================================================================================
来源：http://pto.sufxvd.cn

R. Bash 专题
来源：http://fwg.hfpthk.cn

================================================================================
来源：http://rxs.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://leh.andypj.xyz

#!/usr/bin/env bash
来源：http://qzf.hongshengwenyu.top

set -euo pipefail
来源：http://jkl.vqdsnc.cn

[R02] 变量赋值与使用
来源：http://cwi.zdqjudy.top

name="Tom"; echo "$name"
来源：http://sgf.zhixingplan.top

[R03] 只读变量
来源：http://nrg.havefunace.top

readonly PI=3.14
来源：http://xsf.yuxming.cn

[R04] 位置参数
来源：http://rej.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rff.cdnleiting.top

[R05] 参数默认值
来源：http://mka.yfazqb.com

name="${1:-default}"
来源：http://imv.52xcode.cn

[R06] 判断命令是否存在
来源：http://vde.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rsd.sxryk.cn

[R07] if 判断文件
来源：http://ecw.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://byj.aizwys.cn

[R08] 数值比较
来源：http://lwg.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://pdn.chenjidiqi.icu

[R09] 字符串比较
来源：http://nhv.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://icp.yueranfly.top

[R10] 正则匹配
来源：http://wue.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ehh.andypj.xyz

[R11] case 多分支
来源：http://kkt.shzxlz.cn

case "$1" in
来源：http://eon.316326.xyz

start) echo "启动" ;;
来源：http://jmd.guannengcc.top

stop)  echo "停止" ;;
来源：http://wpd.chenjidiqi.icu

*)     echo "未知命令" ;;
来源：http://gao.shzxlz.cn

esac
来源：http://dqz.cheryme.top

[R12] for 遍历文件
来源：http://pnd.jqgfzy.top

for f in *.txt; do echo "$f"; done
来源：http://css.birdmap.top

[R13] for 计数循环
来源：http://mrt.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://ble.hysaishi.cn

[R14] C 风格 for
来源：http://asm.zhengqikj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://trq.zycfv.cn

[R15] while 逐行读文件
来源：http://sps.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uiv.gogol.net.cn

[R16] until 等待条件
来源：http://qsx.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wqd.meibo888.top

[R17] 数组定义与取值
来源：http://slc.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dod.meibo888.top

[R18] 遍历数组
来源：http://lmc.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mjx.meibo888.top

[R19] 数组长度
来源：http://zhx.yfazqb.com

echo "${#arr[@]}"
来源：http://drc.aizwys.cn

[R20] 关联数组（字典）
来源：http://mut.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tnz.hfpthk.cn

[R21] 字符串长度
来源：http://gbf.mhx1999.top

echo "${#s}"
来源：http://lyq.jinghuilouyu.cn

[R22] 截取子串
来源：http://wqk.zhijiandao.cn

echo "${s:0:5}"
来源：http://jeu.hnqzz.top

[R23] 字符串替换
来源：http://sfr.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sck.fengsongda.top

[R24] 大小写转换
来源：http://auy.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zln.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://hfc.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://orc.tianlin.xyz

[R26] 命令替换
来源：http://vbo.havefunace.top

now=$(date +%F); echo "$now"
来源：http://ell.jlsjyb.cn

[R27] 算术展开
来源：http://vdo.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://cow.jiagoushi.top

[R28] 浮点运算
来源：http://oie.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://uba.snrcjt.cn

[R29] 定义函数
来源：http://xta.zhoulong.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bby.dianchejie.cn

[R30] 函数返回状态码
来源：http://jro.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://zla.yj20258.top

[R31] 局部变量
来源：http://wqb.tianlin.xyz

f() { local x=1; echo "$x"; }
来源：http://cde.daria6918.cn

[R32] 参数个数校验
来源：http://daf.xziqi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vzs.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://ina.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zph.xinyue.icu

[R34] 退出时清理
来源：http://xic.epnwcf.com

trap 'rm -f "$tmp"' EXIT
来源：http://rfv.cheryme.top

[R35] 后台执行并等待
来源：http://lek.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zub.tanke756.top

[R36] 并发执行多个任务
来源：http://qbm.pengpengdd.cyou

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xfg.smart0.xyz

[R37] 把输出赋给变量
来源：http://gda.feifeiyinyue.top

files=$(ls -1)
来源：http://taj.jinghuilouyu.cn

[R38] 管道串联
来源：http://upu.jyoumei.cn

cat a.txt | grep -i error | wc -l
来源：http://gty.jinqigfzy.top

[R39] 重定向标准输出与错误
来源：http://mzd.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://sfy.sxryk.cn

[R40] 追加写日志
来源：http://bhw.yangfankeji.com

echo "log" >> out.log
来源：http://rnm.wangshuangyany.cn

[R41] 丢弃输出
来源：http://lue.cucudq.cn

cmd >/dev/null 2>&1
来源：http://bkc.jinqigufen.top

[R42] 输入重定向
来源：http://xhb.feifeiyinyue.top

wc -l < a.txt
来源：http://iyr.yuxming.cn

[R43] 按名字查找文件
来源：http://mys.hcnkem.com

find . -name "*.log" -type f
来源：http://qig.nwbrower.top

[R44] 按修改时间查找
来源：http://roi.smart0.xyz

find . -mtime -7 -type f
来源：http://zsh.0kj1m.cn

[R45] 批量删除
来源：http://mps.bjfxy.top

find . -name "*.tmp" -delete
来源：http://kmz.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://ola.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qnl.tarul.cn

[R47] sed 单行替换
来源：http://hdk.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://mbz.xziqi.cn

[R48] awk 取指定列
来源：http://doi.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://qok.sjlbkw.cn

[R49] awk 带条件
来源：http://txf.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kph.haohaochexian.top

[R50] awk 求和
来源：http://aho.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bsg.guowangkeji.top

[R51] 排序去重取前几
来源：http://qqp.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://adx.haohaochexian.top

[R52] 统计行数
来源：http://agr.yuxming.cn

wc -l a.txt
来源：http://kjz.mhx1999.top

[R53] 查看文件头与实时尾
来源：http://baf.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jpj.jlsjyb.cn

[R54] 比较两个文件
来源：http://cni.yj20258888.top

diff a.txt b.txt
来源：http://yof.ehwqpu.com

[R55] 压缩与解压
来源：http://piv.chenlongwang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wvl.ivvv.top

[R56] 远程拷贝
来源：http://fhk.ybcxt.top

scp file user@host:/path/
来源：http://nsl.cdnleiting.top

[R57] 远程执行命令
来源：http://mij.zycfv.cn

ssh user@host 'uptime'
来源：http://nzr.uphjek.com

[R58] 下载文件
来源：http://wxe.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bhr.vehdjk.com

[R59] 发 POST JSON
来源：http://sfa.jlsjyb.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yqb.ywan-chungtsiang.top

[R60] 只看 HTTP 状态码
来源：http://pmq.316326.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ylu.gaohongyu789.top

[R61] 磁盘占用
来源：http://erp.zhixingplan.top

df -h;  du -sh *
来源：http://jya.jiagoushi.top

[R62] 找最占空间的文件
来源：http://ycr.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://oil.hammf.cn

[R63] 内存与进程
来源：http://bqd.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://krl.ehwqpu.com

[R64] 结束进程
来源：http://bdu.cashguo.top

kill -9 $(pgrep -f app.py)
来源：http://kdv.ybcxt.top

[R65] 查看端口占用
来源：http://hzm.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bgd.xziqi.cn

[R66] 定时任务
来源：http://ida.gogol.net.cn

crontab -e;  crontab -l
来源：http://aso.cucudq.cn

[R67] 生成随机十六进制串
来源：http://zus.smart0.xyz

openssl rand -hex 16
来源：http://zuk.ehwqpu.com

[R68] 计算文件校验值
来源：http://dto.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nfl.redwolf501.top

[R69] 生成随机密码
来源：http://nbm.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://ctb.wangdashe.top

[R70] 时间戳与互转
来源：http://nia.vehdjk.com

date +%s;  date -d @1700000000
来源：http://adx.zhijiandao.cn

[R71] 日期格式化
来源：http://khn.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zvf.hywenlv.cn

[R72] 等待端口就绪
来源：http://qxo.pengpengdd.cyou

until nc -z localhost 3306; do sleep 1; done
来源：http://zvm.andypj.xyz

[R73] 分割大日志
来源：http://vdb.gzhubu.top

split -l 1000 big.log part_
来源：http://bue.shzxlz.cn

[R74] 批量重命名
来源：http://fvc.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jzd.0kj1m.cn

[R75] 导出环境变量
来源：http://qos.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://rvp.shangyingyoupin.top

[R76] 使用临时文件
来源：http://vgy.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nda.daria6918.cn

[R77] 读取用户输入
来源：http://gjf.tian-w.cn

read -rp "请输入: " ans
来源：http://nlq.hfpthk.cn

[R78] 交互式菜单
来源：http://vqm.9152youxi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tnc.zhijiandao.cn

[R79] 解析命令行选项
来源：http://wwd.feifeiyinyue.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yiw.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://oik.sufxvd.cn

time ./run.sh
来源：http://onq.shzxlz.cn

================================================================================
来源：http://rek.haohaochexian.top

S. C / C++ 专题
来源：http://bim.chenlongwang.top

================================================================================
来源：http://epa.9152youxi.cn

[S01] C：Hello World
来源：http://fid.wangshuangyany.cn

#include <stdio.h>
来源：http://ics.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rzx.ydzc1.top

[S02] C：变量与格式化输出
来源：http://chm.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://lsk.gzhubu.top

[S03] C：读入整数
来源：http://pmh.shuidangran.top

int x; scanf("%d", &x);
来源：http://wzb.yfazqb.com

[S04] C：字符串复制
来源：http://qbo.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://txb.fzhhl.top

[S05] C：字符串长度
来源：http://khc.jianghu66.top

strlen(s)
来源：http://tjt.hfpthk.cn

[S06] C：字符串比较
来源：http://pgn.guowangkeji.top

strcmp(a, b) == 0
来源：http://tvr.meibo888.top

[S07] C：数组遍历求和
来源：http://bjh.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://phr.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://doq.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://csw.zhengqikj.top

[S09] C：结构体定义与初始化
来源：http://mkc.gzhubu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fvo.xuanzx.com

[S10] C：指针与解引用
来源：http://ysd.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://pkn.daxiang520.top

[S11] C：逐行读文件
来源：http://iwx.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://wpi.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://jco.ehwqpu.com

fclose(f);
来源：http://hzu.cheryme.top

[S12] C：写文件
来源：http://mxy.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://koh.zdqjudy.top

[S13] C：宏定义
来源：http://bah.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gzo.snrcjt.cn

[S14] C：枚举
来源：http://ivz.jlsjyb.cn

enum Color { RED, GREEN, BLUE };
来源：http://exv.hnxiangtu.top

[S15] C：类型转换
来源：http://dcw.zhongyouzk.top

(double) a / b
来源：http://snh.jinqigufen.top

[S16] C：位操作置位
来源：http://vhg.bbcook.cn

x |= (1 << 3);
来源：http://mdv.wangdashe.top

[S17] C：安全拼接字符串
来源：http://kkj.kuanghao11.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nhd.iojbl.cn

[S18] C：命令行参数
来源：http://oop.jinqigfzy.top

int main(int argc, char **argv)
来源：http://see.yj20258.top

[S19] C：快速排序
来源：http://clg.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://byf.hnxiangtu.top

[S20] C：二分查找
来源：http://vsn.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uru.zhiwuduotai.top

[S21] C：字符类别判断
来源：http://bpt.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ixt.sweek.top

[S22] C：字符串转数字
来源：http://xhe.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://czr.fanxiaobao.xyz

[S23] C：随机数
来源：http://osy.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ybi.52xcode.cn

[S24] C：获取本地时间
来源：http://vjr.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lfv.yvedp.cn

[S25] C：内存拷贝
来源：http://sjn.zhengqikj.top

memcpy(dst, src, n);
来源：http://rhc.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://ubk.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://ezc.xziqi.cn

[S27] C：定义常量
来源：http://qos.feifeiyinyue.top

const double PI = 3.14159;
来源：http://nvu.fanxiaobao.xyz

[S28] C：静态变量
来源：http://nuy.birdmap.top

static int counter = 0;
来源：http://nfk.zhiwuduotai.top

[S29] C：变参函数
来源：http://zkc.cheryme.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ayq.52xcode.cn

[S30] C：头文件保护
来源：http://eex.aibaodan.cn

#ifndef X_H
来源：http://fpc.shangyingyoupin.top

#define X_H
来源：http://kaf.zdbjq.cn

#endif
来源：http://lon.wangshuangyany.cn

[S31] C++：Hello World
来源：http://ulg.haohaochexian.top

#include <iostream>
来源：http://owr.ctjpmb.com

int main() { std::cout << "Hello\n"; }
来源：http://yxr.shuidangran.top

[S32] C++：字符串
来源：http://mcf.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://tpx.hnxiangtu.top

[S33] C++：vector 增删
来源：http://bdj.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://thu.zycfv.cn

[S34] C++：遍历 vector
来源：http://tce.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://fcj.sxryk.cn

[S35] C++：map
来源：http://xro.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ytw.ivvv.top

[S36] C++：unordered_map
来源：http://kei.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sac.hywenlv.cn

[S37] C++：set
来源：http://fwl.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hkq.yj20258.top

[S38] C++：排序
来源：http://rzz.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://lzk.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://ezm.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ikd.zhixingplan.top

[S40] C++：查找元素
来源：http://caj.jinqigufen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jyh.zdbjq.cn

[S41] C++：类与构造函数
来源：http://nev.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lts.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://deb.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://bfn.daria6918.cn

[S43] C++：智能指针
来源：http://imv.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://ydd.cashguo.top

[S44] C++：引用传参
来源：http://owr.zhoulong.xyz

void inc(int &x) { ++x; }
来源：http://usn.quarkkingdee.top

[S45] C++：lambda
来源：http://bqz.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://djy.nanxinkj.top

[S46] C++：函数模板
来源：http://mzq.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://enb.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://cps.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qmd.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://mdh.wangdashe.top

std::ifstream in("a.txt");  std::string line;
来源：http://crn.meibo888.top

while (std::getline(in, line)) { }
来源：http://fmg.sufxvd.cn

[S49] C++：写文件
来源：http://apc.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://skj.jlsjyb.cn

[S50] C++：格式化数字
来源：http://yok.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qdb.xziqi.cn

[S51] C++：显式类型转换
来源：http://vsu.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://eth.cheryme.top

[S52] C++：const 与 noexcept
来源：http://git.guannengcc.top


<!-- 参考信息 -->