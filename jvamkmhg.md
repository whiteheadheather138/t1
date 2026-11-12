代发 wailian999

[Q84] 去除首尾空格
来源：http://bnd.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://ihp.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://dwe.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://krk.chenlongwang.top

[Q86] 读取 JSON 字段
来源：http://hpd.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aus.yj20258.top

[Q87] JSON 字段做条件
来源：http://sns.c1oappe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cuz.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://sbz.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eyf.dianchejie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jpp.xziqi.cn

[Q89] 判断表是否存在
来源：http://yio.jinqigufen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cdq.gaohongyu789.top

[Q90] 生成序号列
来源：http://whk.xingfuxueyuan.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eli.yvedp.cn

================================================================================
来源：http://fsl.daria6918.cn

R. Bash 专题
来源：http://lti.pengpengdd.cyou

================================================================================
来源：http://veu.gotoacloud.top

[R01] shebang 与严格模式
来源：http://hsb.epnwcf.com

#!/usr/bin/env bash
来源：http://mpy.yuxming.cn

set -euo pipefail
来源：http://tct.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://qxq.shuidangran.top

name="Tom"; echo "$name"
来源：http://nxd.yangfankeji.com

[R03] 只读变量
来源：http://xwe.zhijiandao.cn

readonly PI=3.14
来源：http://yoi.zhiwuduotai.top

[R04] 位置参数
来源：http://csv.jqgufenzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lpg.chenzaomai.com

[R05] 参数默认值
来源：http://hft.9152youxi.cn

name="${1:-default}"
来源：http://xfs.aibaodan.cn

[R06] 判断命令是否存在
来源：http://xgj.zhaomingkeji.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gng.daxiang520.top

[R07] if 判断文件
来源：http://dgn.havefunace.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bqv.epnwcf.com

[R08] 数值比较
来源：http://jkw.zhoulong.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://mpa.hongshengwenyu.top

[R09] 字符串比较
来源：http://sed.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cnm.daria6918.cn

[R10] 正则匹配
来源：http://ees.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gss.yanxiufei.cn

[R11] case 多分支
来源：http://ymy.guannengcc.top

case "$1" in
来源：http://tdg.zdqjudy.top

start) echo "启动" ;;
来源：http://iei.zhengqikj.top

stop)  echo "停止" ;;
来源：http://myi.wangshuangyany.cn

*)     echo "未知命令" ;;
来源：http://eqt.yvedp.cn

esac
来源：http://vxv.cashguo.top

[R12] for 遍历文件
来源：http://zwt.nanxuanxn.top

for f in *.txt; do echo "$f"; done
来源：http://mre.316326.xyz

[R13] for 计数循环
来源：http://cye.xziqi.cn

for i in {1..10}; do echo "$i"; done
来源：http://jvu.meibo888.top

[R14] C 风格 for
来源：http://zks.yanxiufei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wob.gaohongyu789.top

[R15] while 逐行读文件
来源：http://bgi.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bkc.shanyushiyangtech.top

[R16] until 等待条件
来源：http://hqp.shanyushiyangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cvs.smart0.xyz

[R17] 数组定义与取值
来源：http://wha.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://umy.zhaomingkeji.xyz

[R18] 遍历数组
来源：http://wml.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://maj.fehbvm.com

[R19] 数组长度
来源：http://imq.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://btu.ybcxt.top

[R20] 关联数组（字典）
来源：http://jmv.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fwh.mhx1999.top

[R21] 字符串长度
来源：http://ita.sweek.top

echo "${#s}"
来源：http://ezf.chenzaomai.com

[R22] 截取子串
来源：http://oes.pengpengdd.cyou

echo "${s:0:5}"
来源：http://eru.pycfn.com

[R23] 字符串替换
来源：http://rkl.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lgj.cqqwz.cn

[R24] 大小写转换
来源：http://wnk.hcnkem.com

echo "${s^^}"; echo "${s,,}"
来源：http://yml.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://hms.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gva.hcnkem.com

[R26] 命令替换
来源：http://jeu.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://urj.xinyue.icu

[R27] 算术展开
来源：http://sfs.daxiang520.top

echo $((1 + 2 * 3))
来源：http://syx.zdbjq.cn

[R28] 浮点运算
来源：http://map.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://enr.c1oappe.top

[R29] 定义函数
来源：http://wfs.redwolf501.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ulk.sxryk.cn

[R30] 函数返回状态码
来源：http://hbz.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://gfu.quarkkingdee.top

[R31] 局部变量
来源：http://uia.zhoulong.xyz

f() { local x=1; echo "$x"; }
来源：http://thg.ctjpmb.com

[R32] 参数个数校验
来源：http://pbh.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://scf.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://vxq.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cjz.ppjwa.cn

[R34] 退出时清理
来源：http://fqc.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://amv.uphjek.com

[R35] 后台执行并等待
来源：http://wtg.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://med.redwolf501.top

[R36] 并发执行多个任务
来源：http://eya.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cwk.aizwys.cn

[R37] 把输出赋给变量
来源：http://oiw.hysaishi.cn

files=$(ls -1)
来源：http://zss.zhoulong.xyz

[R38] 管道串联
来源：http://oja.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://kzg.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://gfd.dashuyun.cn

cmd > out.log 2>&1
来源：http://zbg.ydzc1.top

[R40] 追加写日志
来源：http://xcm.xinyue.icu

echo "log" >> out.log
来源：http://xny.jlsjyb.cn

[R41] 丢弃输出
来源：http://cbr.fzhhl.top

cmd >/dev/null 2>&1
来源：http://yeh.pycfn.com

[R42] 输入重定向
来源：http://gih.gotoacloud.top

wc -l < a.txt
来源：http://ttd.ppjwa.cn

[R43] 按名字查找文件
来源：http://wrk.gotoacloud.top

find . -name "*.log" -type f
来源：http://tzn.snrcjt.cn

[R44] 按修改时间查找
来源：http://lrv.chenlongwang.top

find . -mtime -7 -type f
来源：http://nlj.jqgfzy.top

[R45] 批量删除
来源：http://urt.sufxvd.cn

find . -name "*.tmp" -delete
来源：http://gtz.zdbjq.cn

[R46] 递归替换文件内容
来源：http://ayx.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ipn.iojbl.cn

[R47] sed 单行替换
来源：http://ytj.zhiwuduotai.top

sed -i 's/foo/bar/g' a.txt
来源：http://zfc.zhengqikj.top

[R48] awk 取指定列
来源：http://zze.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://udx.sjlbkw.cn

[R49] awk 带条件
来源：http://vls.jinqigufen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mke.yvedp.cn

[R50] awk 求和
来源：http://cfc.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://zds.yuxming.cn

[R51] 排序去重取前几
来源：http://lpf.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://puk.hammf.cn

[R52] 统计行数
来源：http://wcx.uphjek.com

wc -l a.txt
来源：http://tjg.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://lva.svipenyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hqr.bbcook.cn

[R54] 比较两个文件
来源：http://oud.zhongyouzk.top

diff a.txt b.txt
来源：http://elt.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://mjw.sweek.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://piz.uphjek.com

[R56] 远程拷贝
来源：http://jwo.redwolf501.top

scp file user@host:/path/
来源：http://nhq.fktsv.cn

[R57] 远程执行命令
来源：http://mak.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://ujh.ybcxt.top

[R58] 下载文件
来源：http://xzs.zhixingplan.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hvs.smart0.xyz

[R59] 发 POST JSON
来源：http://tar.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mcg.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://nrt.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zmc.pengpengdd.cyou

[R61] 磁盘占用
来源：http://ngm.tanke756.top

df -h;  du -sh *
来源：http://cqk.sweek.top

[R62] 找最占空间的文件
来源：http://qom.pycfn.com

du -ah . | sort -rh | head -10
来源：http://rpe.ivvv.top

[R63] 内存与进程
来源：http://wmf.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://cav.jinqigfzy.top

[R64] 结束进程
来源：http://oul.jiagoushi.top

kill -9 $(pgrep -f app.py)
来源：http://gmv.chenzaomai.com

[R65] 查看端口占用
来源：http://zsj.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bhm.jqgfzy.top

[R66] 定时任务
来源：http://yxu.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://vzn.yuxming.cn

[R67] 生成随机十六进制串
来源：http://lsq.ybcxt.top

openssl rand -hex 16
来源：http://emp.sufxvd.cn

[R68] 计算文件校验值
来源：http://blm.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://lwn.yongpay.top

[R69] 生成随机密码
来源：http://iyh.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://zsp.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://ttx.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://yop.fktsv.cn

[R71] 日期格式化
来源：http://pmf.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://onw.316326.xyz

[R72] 等待端口就绪
来源：http://bqq.yfazqb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://pnj.shanyushiyangtech.top

[R73] 分割大日志
来源：http://xda.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://cut.gzhubu.top

[R74] 批量重命名
来源：http://syt.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://khz.iojbl.cn

[R75] 导出环境变量
来源：http://vnt.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://hac.havefunace.top

[R76] 使用临时文件
来源：http://mbo.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://llr.hnxiangtu.top

[R77] 读取用户输入
来源：http://nzi.9152youxi.cn

read -rp "请输入: " ans
来源：http://jdz.9152youxi.cn

[R78] 交互式菜单
来源：http://bln.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://vzp.gzhubu.top

[R79] 解析命令行选项
来源：http://xbl.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://deg.ybcxt.top

[R80] 查看脚本执行耗时
来源：http://ywa.hfpthk.cn

time ./run.sh
来源：http://cuv.52xcode.cn

================================================================================
来源：http://ljk.xylfe.cn

S. C / C++ 专题
来源：http://mqn.sjlbkw.cn

================================================================================
来源：http://sar.hywenlv.cn

[S01] C：Hello World
来源：http://jlr.ivvv.top

#include <stdio.h>
来源：http://uhd.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://grw.nwbrower.top

[S02] C：变量与格式化输出
来源：http://vdk.shanyushiyangkeji.top

int a = 10; printf("%d\n", a);
来源：http://awz.ydjk.org.cn

[S03] C：读入整数
来源：http://zwl.ydzc1.top

int x; scanf("%d", &x);
来源：http://ahd.gaohongyu789.top

[S04] C：字符串复制
来源：http://dig.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rcr.kuanghao11.cn

[S05] C：字符串长度
来源：http://thd.316326.xyz

strlen(s)
来源：http://avl.9152youxi.cn

[S06] C：字符串比较
来源：http://ckx.jqgfzy.top

strcmp(a, b) == 0
来源：http://hls.smart0.xyz

[S07] C：数组遍历求和
来源：http://kcb.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rhq.yj202588.top

[S08] C：动态内存分配与释放
来源：http://vhe.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vnt.gogol.net.cn

[S09] C：结构体定义与初始化
来源：http://ptv.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cnh.tianlin.xyz

[S10] C：指针与解引用
来源：http://odz.xziqi.cn

int *p = &a;  *p = 5;
来源：http://msq.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://qoc.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://nvu.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fyd.zycfv.cn

fclose(f);
来源：http://rnc.dianchejie.cn

[S12] C：写文件
来源：http://snl.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://knt.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://put.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rgv.redwolf501.top

[S14] C：枚举
来源：http://jjf.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://fjy.fengsongda.top

[S15] C：类型转换
来源：http://gcr.chenlongwang.top

(double) a / b
来源：http://tzi.jianghu66.top

[S16] C：位操作置位
来源：http://xfd.tanke756.top

x |= (1 << 3);
来源：http://xdy.sweek.top

[S17] C：安全拼接字符串
来源：http://lwh.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wpu.guannengcc.top

[S18] C：命令行参数
来源：http://tag.zhijiandao.cn

int main(int argc, char **argv)
来源：http://lqz.sufxvd.cn

[S19] C：快速排序
来源：http://fml.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://igp.yongpay.top

[S20] C：二分查找
来源：http://hqc.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zcj.vehdjk.com

[S21] C：字符类别判断
来源：http://ecg.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jnc.cheryme.top

[S22] C：字符串转数字
来源：http://kqc.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bez.nwbrower.top

[S23] C：随机数
来源：http://wfs.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cpc.shzxlz.cn

[S24] C：获取本地时间
来源：http://qxc.zhengqikj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nai.yfazqb.com

[S25] C：内存拷贝
来源：http://lbq.jianghu66.top

memcpy(dst, src, n);
来源：http://piw.fanxiaobao.xyz

[S26] C：内存清零
来源：http://jrt.xuanzx.com

memset(a, 0, sizeof a);
来源：http://jiu.havefunace.top

[S27] C：定义常量
来源：http://xpl.cqqwz.cn

const double PI = 3.14159;
来源：http://yqj.hcnkem.com

[S28] C：静态变量
来源：http://zbz.hnxiangtu.top

static int counter = 0;
来源：http://oeb.fzhhl.top

[S29] C：变参函数
来源：http://qfd.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lzl.9152youxi.cn

[S30] C：头文件保护
来源：http://bet.redwolf501.top

#ifndef X_H
来源：http://hrh.ydjk.org.cn

#define X_H
来源：http://tbc.xylfe.cn

#endif
来源：http://aqt.aizwys.cn

[S31] C++：Hello World
来源：http://tyx.bbcook.cn

#include <iostream>
来源：http://dnm.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://qws.chenjidiqi.icu

[S32] C++：字符串
来源：http://uiv.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://cxx.xuanzx.com

[S33] C++：vector 增删
来源：http://oeh.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qia.yvedp.cn

[S34] C++：遍历 vector
来源：http://xaz.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://dfi.jinghuilouyu.cn

[S35] C++：map
来源：http://gii.xuanzx.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gav.hywenlv.cn

[S36] C++：unordered_map
来源：http://ylr.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mfk.zdbjq.cn

[S37] C++：set
来源：http://smw.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gwq.shuidangran.top

[S38] C++：排序
来源：http://owq.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://ydv.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://twf.zhixingplan.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bsj.pycfn.com

[S40] C++：查找元素
来源：http://eag.svipenyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lki.bjfxy.top

[S41] C++：类与构造函数
来源：http://jip.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tjk.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://bil.jiagoushi.top

class B : public Base { public: void f() override {} };
来源：http://crn.gaohongyu789.top

[S43] C++：智能指针
来源：http://bls.gaohongyu789.top

auto p = std::make_unique<int>(5);
来源：http://ldd.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://ofz.sxryk.cn

void inc(int &x) { ++x; }
来源：http://ggm.nwbrower.top

[S45] C++：lambda
来源：http://oha.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://nuu.c1oappe.top

[S46] C++：函数模板
来源：http://qlv.hywenlv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zed.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://qep.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lpd.cqqwz.cn

[S48] C++：逐行读文件
来源：http://eld.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://ore.bjfxy.top

while (std::getline(in, line)) { }
来源：http://eeb.xziqi.cn

[S49] C++：写文件
来源：http://idr.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yeo.vehdjk.com

[S50] C++：格式化数字
来源：http://pud.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uae.hysaishi.cn

[S51] C++：显式类型转换
来源：http://mwd.nanxuanxn.top

static_cast<double>(a) / b
来源：http://ukp.zdbjq.cn

[S52] C++：const 与 noexcept
来源：http://itg.yfazqb.com

int size() const noexcept { return n_; }
来源：http://qou.yuanzhike.top

[S53] C++：移动语义
来源：http://urm.gzhubu.top

std::vector<int> w = std::move(v);
来源：http://zwy.shzxlz.cn

[S54] C++：异常处理
来源：http://yco.cashguo.top


<!-- 参考信息 -->