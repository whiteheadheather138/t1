代发 wailian999

[Q82] 字符长度与字节长度
来源：http://nhr.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pos.uphjek.com

[Q83] 大小写转换
来源：http://vht.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://etm.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://yxe.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://zfy.fktsv.cn

[Q85] 数值取整
来源：http://yll.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jvc.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://qua.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tqy.tarul.cn

[Q87] JSON 字段做条件
来源：http://oga.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bzi.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://ebn.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xdp.zhixingplan.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gxj.guowangkeji.top

[Q89] 判断表是否存在
来源：http://ehh.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oqm.cashguo.top

[Q90] 生成序号列
来源：http://oax.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rdl.cheryme.top

================================================================================
来源：http://elv.xziqi.cn

R. Bash 专题
来源：http://qdw.feifeiyinyue.top

================================================================================
来源：http://con.hnxiangtu.top

[R01] shebang 与严格模式
来源：http://gua.yfazqb.com

#!/usr/bin/env bash
来源：http://owg.gzhubu.top

set -euo pipefail
来源：http://rie.fktsv.cn

[R02] 变量赋值与使用
来源：http://lrv.xziqi.cn

name="Tom"; echo "$name"
来源：http://inu.yanxiufei.cn

[R03] 只读变量
来源：http://wtw.yangfankeji.com

readonly PI=3.14
来源：http://yhh.hnxiangtu.top

[R04] 位置参数
来源：http://nhd.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zkb.zhoulong.xyz

[R05] 参数默认值
来源：http://slp.yfazqb.com

name="${1:-default}"
来源：http://qzo.iojbl.cn

[R06] 判断命令是否存在
来源：http://itt.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bgz.fzhhl.top

[R07] if 判断文件
来源：http://sbh.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nwi.nanxinkj.top

[R08] 数值比较
来源：http://tbg.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rfw.52xcode.cn

[R09] 字符串比较
来源：http://gcj.hesvh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wrl.cucudq.cn

[R10] 正则匹配
来源：http://cbe.aibaodan.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wki.zdqjudy.top

[R11] case 多分支
来源：http://haw.meibo888.top

case "$1" in
来源：http://hiy.hammf.cn

start) echo "启动" ;;
来源：http://ixo.mhx1999.top

stop)  echo "停止" ;;
来源：http://uqk.guannengcc.top

*)     echo "未知命令" ;;
来源：http://bwz.ivvv.top

esac
来源：http://qrt.hongshengwenyu.top

[R12] for 遍历文件
来源：http://zhx.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://iwo.ctjpmb.com

[R13] for 计数循环
来源：http://bhs.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://ris.sjlbkw.cn

[R14] C 风格 for
来源：http://dbo.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ymz.yj202588.top

[R15] while 逐行读文件
来源：http://gfj.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bts.sysykeji.top

[R16] until 等待条件
来源：http://var.mhx1999.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lad.jinyuanbaomall.cn

[R17] 数组定义与取值
来源：http://kcd.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://qfg.cashguo.top

[R18] 遍历数组
来源：http://cov.jqgufenzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hmq.wangdashe.top

[R19] 数组长度
来源：http://qsn.zycfv.cn

echo "${#arr[@]}"
来源：http://vtm.ivvv.top

[R20] 关联数组（字典）
来源：http://jhd.yanxiufei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qrq.bjfxy.top

[R21] 字符串长度
来源：http://unf.guannengcc.top

echo "${#s}"
来源：http://zze.vqdsnc.cn

[R22] 截取子串
来源：http://pjf.yj202588.top

echo "${s:0:5}"
来源：http://cxx.fktsv.cn

[R23] 字符串替换
来源：http://uny.nanxuanxn.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rnr.guowangkeji.top

[R24] 大小写转换
来源：http://lzb.hongshengwenyu.top

echo "${s^^}"; echo "${s,,}"
来源：http://gbm.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://ivs.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://czs.meibo888.top

[R26] 命令替换
来源：http://mji.chenlongwang.top

now=$(date +%F); echo "$now"
来源：http://jzl.gzhubu.top

[R27] 算术展开
来源：http://wwc.gogol.net.cn

echo $((1 + 2 * 3))
来源：http://qnw.gotoacloud.top

[R28] 浮点运算
来源：http://ber.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://wec.chenjidiqi.icu

[R29] 定义函数
来源：http://dez.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yja.jinqigufen.top

[R30] 函数返回状态码
来源：http://cuh.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://fzp.zhoulong.xyz

[R31] 局部变量
来源：http://llo.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://kjr.xuetiantiany.cn

[R32] 参数个数校验
来源：http://xaz.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kah.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://ist.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lpj.yj20258.top

[R34] 退出时清理
来源：http://kwe.snrcjt.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pqv.mhx1999.top

[R35] 后台执行并等待
来源：http://buk.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mtz.tarul.cn

[R36] 并发执行多个任务
来源：http://vhc.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bjn.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://bni.xinyue.icu

files=$(ls -1)
来源：http://eta.aizwys.cn

[R38] 管道串联
来源：http://ktb.tianlin.xyz

cat a.txt | grep -i error | wc -l
来源：http://cvp.hnqzz.top

[R39] 重定向标准输出与错误
来源：http://wic.shanyushiyangtech.top

cmd > out.log 2>&1
来源：http://ift.guowangkeji.top

[R40] 追加写日志
来源：http://siu.bjfxy.top

echo "log" >> out.log
来源：http://rag.feifeiyinyue.top

[R41] 丢弃输出
来源：http://hkc.yueranfly.top

cmd >/dev/null 2>&1
来源：http://ypf.zhijiandao.cn

[R42] 输入重定向
来源：http://dyg.mhx1999.top

wc -l < a.txt
来源：http://icg.sufxvd.cn

[R43] 按名字查找文件
来源：http://uve.yj20258.top

find . -name "*.log" -type f
来源：http://gsl.nanxuanxn.top

[R44] 按修改时间查找
来源：http://fbn.316326.xyz

find . -mtime -7 -type f
来源：http://psv.andypj.xyz

[R45] 批量删除
来源：http://vpw.fengsongda.top

find . -name "*.tmp" -delete
来源：http://kwm.ctjpmb.com

[R46] 递归替换文件内容
来源：http://ydi.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vwz.zhengqikj.top

[R47] sed 单行替换
来源：http://bep.guannengcc.top

sed -i 's/foo/bar/g' a.txt
来源：http://kmp.jiagoushi.top

[R48] awk 取指定列
来源：http://esn.xuanzx.com

awk '{print $1, $3}' a.txt
来源：http://fth.zhixingplan.top

[R49] awk 带条件
来源：http://omx.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hid.zhixingplan.top

[R50] awk 求和
来源：http://clk.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://adi.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://lsu.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://xql.dashuyun.cn

[R52] 统计行数
来源：http://qnk.gotoacloud.top

wc -l a.txt
来源：http://gag.yueranfly.top

[R53] 查看文件头与实时尾
来源：http://loz.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wsj.hfpthk.cn

[R54] 比较两个文件
来源：http://ube.yj202588.top

diff a.txt b.txt
来源：http://hbi.jlsjyb.cn

[R55] 压缩与解压
来源：http://nxf.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wff.jinqigufen.top

[R56] 远程拷贝
来源：http://cqq.shuidangran.top

scp file user@host:/path/
来源：http://xkp.ivvv.top

[R57] 远程执行命令
来源：http://rhr.cucudq.cn

ssh user@host 'uptime'
来源：http://vxl.cucudq.cn

[R58] 下载文件
来源：http://sck.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://akx.andypj.xyz

[R59] 发 POST JSON
来源：http://bsj.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fqy.ywan-chungtsiang.top

[R60] 只看 HTTP 状态码
来源：http://nuy.c1oappe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iyq.nwbrower.top

[R61] 磁盘占用
来源：http://dxj.hnxiangtu.top

df -h;  du -sh *
来源：http://buv.jiagoushi.top

[R62] 找最占空间的文件
来源：http://jrn.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://cib.nwbrower.top

[R63] 内存与进程
来源：http://mrr.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://xgm.wangdashe.top

[R64] 结束进程
来源：http://wdb.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://lag.hnqzz.top

[R65] 查看端口占用
来源：http://xwk.haohaochexian.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cvh.sjlbkw.cn

[R66] 定时任务
来源：http://lwv.hcnkem.com

crontab -e;  crontab -l
来源：http://abj.c1oappe.top

[R67] 生成随机十六进制串
来源：http://kld.c1oappe.top

openssl rand -hex 16
来源：http://exa.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://xie.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://rto.jlsjyb.cn

[R69] 生成随机密码
来源：http://ghi.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://liy.cashguo.top

[R70] 时间戳与互转
来源：http://fnt.sweek.top

date +%s;  date -d @1700000000
来源：http://vew.sufxvd.cn

[R71] 日期格式化
来源：http://nga.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jte.aizwys.cn

[R72] 等待端口就绪
来源：http://jtx.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xro.feifeiyinyue.top

[R73] 分割大日志
来源：http://zds.yj202588.top

split -l 1000 big.log part_
来源：http://xqn.pycfn.com

[R74] 批量重命名
来源：http://kmr.yuxming.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dfz.ivvv.top

[R75] 导出环境变量
来源：http://msl.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://hyo.zdqjudy.top

[R76] 使用临时文件
来源：http://sev.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://edn.ydzc1.top

[R77] 读取用户输入
来源：http://qtc.redwolf501.top

read -rp "请输入: " ans
来源：http://wjs.kuanghao11.cn

[R78] 交互式菜单
来源：http://syc.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sxd.iojbl.cn

[R79] 解析命令行选项
来源：http://sdn.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fvl.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://unn.smart0.xyz

time ./run.sh
来源：http://kfm.ehwqpu.com

================================================================================
来源：http://tsf.ydzc1.top

S. C / C++ 专题
来源：http://qjj.feifeiyinyue.top

================================================================================
来源：http://reg.gotoacloud.top

[S01] C：Hello World
来源：http://xjs.wangdashe.top

#include <stdio.h>
来源：http://fkd.epnwcf.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://tfm.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://rcu.bjfxy.top

int a = 10; printf("%d\n", a);
来源：http://pgo.hnqzz.top

[S03] C：读入整数
来源：http://ifn.nwbrower.top

int x; scanf("%d", &x);
来源：http://fll.tianlin.xyz

[S04] C：字符串复制
来源：http://oiv.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qld.pycfn.com

[S05] C：字符串长度
来源：http://hxe.hywenlv.cn

strlen(s)
来源：http://zdx.daria6918.cn

[S06] C：字符串比较
来源：http://phg.bjfxy.top

strcmp(a, b) == 0
来源：http://dwg.fzhhl.top

[S07] C：数组遍历求和
来源：http://lcl.ydzc1.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qhz.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://wgi.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vgi.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://bhb.0kj1m.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nia.hcnkem.com

[S10] C：指针与解引用
来源：http://zlu.vqdsnc.cn

int *p = &a;  *p = 5;
来源：http://mwd.daxiang520.top

[S11] C：逐行读文件
来源：http://mqk.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://sor.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xiy.9152youxi.cn

fclose(f);
来源：http://liy.yuanzhike.top

[S12] C：写文件
来源：http://clo.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://utu.ppjwa.cn

[S13] C：宏定义
来源：http://zns.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nes.tarul.cn

[S14] C：枚举
来源：http://wob.yangfankeji.com

enum Color { RED, GREEN, BLUE };
来源：http://jtg.yj202588.top

[S15] C：类型转换
来源：http://fpj.daria6918.cn

(double) a / b
来源：http://mxp.zdqjudy.top

[S16] C：位操作置位
来源：http://qmu.yfazqb.com

x |= (1 << 3);
来源：http://azd.wangdashe.top

[S17] C：安全拼接字符串
来源：http://lnz.sjlbkw.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uot.xinyue.icu

[S18] C：命令行参数
来源：http://coe.hammf.cn

int main(int argc, char **argv)
来源：http://mnt.chenzaomai.com

[S19] C：快速排序
来源：http://obj.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://cen.xuetiantiany.cn

[S20] C：二分查找
来源：http://lod.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tzp.fehbvm.com

[S21] C：字符类别判断
来源：http://mgi.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ovm.9152youxi.cn

[S22] C：字符串转数字
来源：http://uyo.kuanghao11.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ryh.yanxiufei.cn

[S23] C：随机数
来源：http://hvp.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ksu.hesvh.cn

[S24] C：获取本地时间
来源：http://hpr.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mtv.chenzaomai.com

[S25] C：内存拷贝
来源：http://qny.hnxiangtu.top

memcpy(dst, src, n);
来源：http://hlj.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://bdx.52xcode.cn

memset(a, 0, sizeof a);
来源：http://ntv.zhengqikj.top

[S27] C：定义常量
来源：http://ubs.vehdjk.com

const double PI = 3.14159;
来源：http://ofp.aizwys.cn

[S28] C：静态变量
来源：http://oxf.snrcjt.cn

static int counter = 0;
来源：http://pdh.52xcode.cn

[S29] C：变参函数
来源：http://qlb.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wby.gogol.net.cn

[S30] C：头文件保护
来源：http://fux.tanke756.top

#ifndef X_H
来源：http://tia.jinghuilouyu.cn

#define X_H
来源：http://meb.gogol.net.cn

#endif
来源：http://kuf.quarkkingdee.top

[S31] C++：Hello World
来源：http://yxk.xinyue.icu

#include <iostream>
来源：http://hxa.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://ggx.jqgfzy.top

[S32] C++：字符串
来源：http://etb.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://mug.andypj.xyz

[S33] C++：vector 增删
来源：http://dbm.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nkr.bjfxy.top

[S34] C++：遍历 vector
来源：http://bqp.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://hbw.shangyingyoupin.top

[S35] C++：map
来源：http://sqf.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yol.shzxlz.cn

[S36] C++：unordered_map
来源：http://iyr.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mpz.redwolf501.top

[S37] C++：set
来源：http://fbx.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zih.sweek.top

[S38] C++：排序
来源：http://cfp.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://mvv.hammf.cn

[S39] C++：自定义比较器排序
来源：http://jqd.jqgufenzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lks.meibo888.top

[S40] C++：查找元素
来源：http://axi.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://auf.cheryme.top

[S41] C++：类与构造函数
来源：http://oga.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kbq.fehbvm.com

[S42] C++：继承与虚函数
来源：http://vdj.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://wol.cdnleiting.top

[S43] C++：智能指针
来源：http://kvr.0kj1m.cn

auto p = std::make_unique<int>(5);
来源：http://wlr.svipenyu.cn

[S44] C++：引用传参
来源：http://dnq.hesvh.cn

void inc(int &x) { ++x; }
来源：http://mbr.pengpengdd.cyou

[S45] C++：lambda
来源：http://tfq.aizwys.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zmg.zhoulong.xyz

[S46] C++：函数模板
来源：http://vfc.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://abd.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://uiz.ehwqpu.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pqp.nanxuanxn.top

[S48] C++：逐行读文件
来源：http://dat.quarkkingdee.top

std::ifstream in("a.txt");  std::string line;
来源：http://hzf.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://vir.fengsongda.top

[S49] C++：写文件
来源：http://blm.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dzs.yj202588.top

[S50] C++：格式化数字
来源：http://emm.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://olr.shzxlz.cn

[S51] C++：显式类型转换
来源：http://mbh.xuetiantiany.cn

static_cast<double>(a) / b
来源：http://xnk.yangfankeji.com

[S52] C++：const 与 noexcept
来源：http://cpl.wangshuangyany.cn


<!-- 参考信息 -->