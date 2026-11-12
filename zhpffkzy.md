代发 wailian999

[Q86] 读取 JSON 字段
来源：http://upp.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ljz.snrcjt.cn

[Q87] JSON 字段做条件
来源：http://mlr.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vzd.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://muh.yvedp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cez.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rpf.tarul.cn

[Q89] 判断表是否存在
来源：http://sez.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jfw.dianchejie.cn

[Q90] 生成序号列
来源：http://ldh.xingfuxueyuan.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mqy.nanxuanxn.top

================================================================================
来源：http://ycr.yj20258888.top

R. Bash 专题
来源：http://mhu.zdbjq.cn

================================================================================
来源：http://red.sxryk.cn

[R01] shebang 与严格模式
来源：http://bku.yonumen.top

#!/usr/bin/env bash
来源：http://xfy.zdbjq.cn

set -euo pipefail
来源：http://ywc.cqqwz.cn

[R02] 变量赋值与使用
来源：http://ctj.bjfxy.top

name="Tom"; echo "$name"
来源：http://tpc.fengsongda.top

[R03] 只读变量
来源：http://xgg.fengsongda.top

readonly PI=3.14
来源：http://wgx.c1oappe.top

[R04] 位置参数
来源：http://xte.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kir.yuanzhike.top

[R05] 参数默认值
来源：http://nex.dianchejie.cn

name="${1:-default}"
来源：http://tez.0kj1m.cn

[R06] 判断命令是否存在
来源：http://vip.daxiang520.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gng.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://iai.bbcook.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qod.xuanzx.com

[R08] 数值比较
来源：http://eyp.iojbl.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hsr.tian-w.cn

[R09] 字符串比较
来源：http://kga.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aek.svipenyu.cn

[R10] 正则匹配
来源：http://ljd.vqdsnc.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pog.c1oappe.top

[R11] case 多分支
来源：http://sij.xylfe.cn

case "$1" in
来源：http://lbe.jqgufenzy.top

start) echo "启动" ;;
来源：http://naz.pycfn.com

stop)  echo "停止" ;;
来源：http://apy.iojbl.cn

*)     echo "未知命令" ;;
来源：http://swm.zhixingplan.top

esac
来源：http://gjv.zhoulong.xyz

[R12] for 遍历文件
来源：http://puo.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://hnk.cqqwz.cn

[R13] for 计数循环
来源：http://hdf.bjfxy.top

for i in {1..10}; do echo "$i"; done
来源：http://pjq.cashguo.top

[R14] C 风格 for
来源：http://uri.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eeo.zhijiandao.cn

[R15] while 逐行读文件
来源：http://rgk.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kjb.cdnleiting.top

[R16] until 等待条件
来源：http://yii.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wva.svipenyu.cn

[R17] 数组定义与取值
来源：http://vsd.xuanzx.com

arr=(a b c); echo "${arr[0]}"
来源：http://itz.zhixingplan.top

[R18] 遍历数组
来源：http://xas.yfazqb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rtu.yuxming.cn

[R19] 数组长度
来源：http://tle.hnqzz.top

echo "${#arr[@]}"
来源：http://qfj.gaohongyu789.top

[R20] 关联数组（字典）
来源：http://sml.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lbo.c1oappe.top

[R21] 字符串长度
来源：http://vau.chenzaomai.com

echo "${#s}"
来源：http://yyh.ybcxt.top

[R22] 截取子串
来源：http://qst.redwolf501.top

echo "${s:0:5}"
来源：http://dnx.jianghu66.top

[R23] 字符串替换
来源：http://csw.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nlj.yj202588.top

[R24] 大小写转换
来源：http://ukf.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://let.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://ajh.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kwh.hcnkem.com

[R26] 命令替换
来源：http://vzb.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://byl.hysaishi.cn

[R27] 算术展开
来源：http://okl.daria6918.cn

echo $((1 + 2 * 3))
来源：http://azn.daria6918.cn

[R28] 浮点运算
来源：http://bkk.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://mhc.yongpay.top

[R29] 定义函数
来源：http://pvu.hesvh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sao.fengsongda.top

[R30] 函数返回状态码
来源：http://pec.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://oqc.xuanzx.com

[R31] 局部变量
来源：http://hou.yangfankeji.com

f() { local x=1; echo "$x"; }
来源：http://kak.gaohongyu789.top

[R32] 参数个数校验
来源：http://gdv.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xjs.pycfn.com

[R33] 捕获错误并提示行号
来源：http://jzn.fehbvm.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xkg.zhongyouzk.top

[R34] 退出时清理
来源：http://ngi.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rxi.guowangkeji.top

[R35] 后台执行并等待
来源：http://euy.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hgu.jinyuanbaomall.cn

[R36] 并发执行多个任务
来源：http://nfv.gaohongyu789.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vge.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://xzv.yj202588.top

files=$(ls -1)
来源：http://mxt.zhijiandao.cn

[R38] 管道串联
来源：http://hpc.bjfxy.top

cat a.txt | grep -i error | wc -l
来源：http://vaa.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://kfc.xziqi.cn

cmd > out.log 2>&1
来源：http://ljy.cashguo.top

[R40] 追加写日志
来源：http://nhy.hfpthk.cn

echo "log" >> out.log
来源：http://mbi.hfpthk.cn

[R41] 丢弃输出
来源：http://dyw.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://end.meibo888.top

[R42] 输入重定向
来源：http://gpn.gogol.net.cn

wc -l < a.txt
来源：http://ifc.fehbvm.com

[R43] 按名字查找文件
来源：http://zxd.nwbrower.top

find . -name "*.log" -type f
来源：http://zwj.hesvh.cn

[R44] 按修改时间查找
来源：http://lkc.dianchejie.cn

find . -mtime -7 -type f
来源：http://crc.vehdjk.com

[R45] 批量删除
来源：http://cxr.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://ccz.zhixingplan.top

[R46] 递归替换文件内容
来源：http://rcg.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fgh.zhengqikj.top

[R47] sed 单行替换
来源：http://hil.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zwz.yuxming.cn

[R48] awk 取指定列
来源：http://idj.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://ehx.chenlongwang.top

[R49] awk 带条件
来源：http://ooo.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ajv.zdbjq.cn

[R50] awk 求和
来源：http://pqp.tian-w.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kaz.jyoumei.cn

[R51] 排序去重取前几
来源：http://czi.ehwqpu.com

sort a.txt | uniq -c | sort -rn | head
来源：http://hwr.yongpay.top

[R52] 统计行数
来源：http://ltm.chenzaomai.com

wc -l a.txt
来源：http://qod.fzhhl.top

[R53] 查看文件头与实时尾
来源：http://eod.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rez.svipenyu.cn

[R54] 比较两个文件
来源：http://mqs.yueranfly.top

diff a.txt b.txt
来源：http://ofb.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://rep.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cgb.bbcook.cn

[R56] 远程拷贝
来源：http://ttx.hcnkem.com

scp file user@host:/path/
来源：http://msg.yongpay.top

[R57] 远程执行命令
来源：http://ord.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://dax.shangyingyoupin.top

[R58] 下载文件
来源：http://tee.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gek.cqqwz.cn

[R59] 发 POST JSON
来源：http://mfs.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tgu.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://uot.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://edv.aizwys.cn

[R61] 磁盘占用
来源：http://hys.gotoacloud.top

df -h;  du -sh *
来源：http://pfg.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://sgk.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://dbq.yongpay.top

[R63] 内存与进程
来源：http://fbl.yanxiufei.cn

free -h;  ps aux | grep nginx
来源：http://nue.smart0.xyz

[R64] 结束进程
来源：http://moi.316326.xyz

kill -9 $(pgrep -f app.py)
来源：http://eoi.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://smk.dashuyun.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yhw.zhiwuduotai.top

[R66] 定时任务
来源：http://grd.ctjpmb.com

crontab -e;  crontab -l
来源：http://poh.birdmap.top

[R67] 生成随机十六进制串
来源：http://gpw.ppjwa.cn

openssl rand -hex 16
来源：http://non.hywenlv.cn

[R68] 计算文件校验值
来源：http://qkw.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://smr.kuanghao11.cn

[R69] 生成随机密码
来源：http://xcu.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://kdm.sxryk.cn

[R70] 时间戳与互转
来源：http://pei.aibaodan.cn

date +%s;  date -d @1700000000
来源：http://xow.pengpengdd.cyou

[R71] 日期格式化
来源：http://eyz.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hnq.jiagoushi.top

[R72] 等待端口就绪
来源：http://kni.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ndk.chenlongwang.top

[R73] 分割大日志
来源：http://ezi.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://wmf.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://ouc.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ezs.birdmap.top

[R75] 导出环境变量
来源：http://gjc.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://hns.jlsjyb.cn

[R76] 使用临时文件
来源：http://lpz.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://icy.tian-w.cn

[R77] 读取用户输入
来源：http://gbj.ehwqpu.com

read -rp "请输入: " ans
来源：http://jre.zhijiandao.cn

[R78] 交互式菜单
来源：http://iju.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://brw.chenzaomai.com

[R79] 解析命令行选项
来源：http://mgw.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rhf.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://mzr.uphjek.com

time ./run.sh
来源：http://uyq.cqqwz.cn

================================================================================
来源：http://kiz.fktsv.cn

S. C / C++ 专题
来源：http://hxe.jianghu66.top

================================================================================
来源：http://fjz.epnwcf.com

[S01] C：Hello World
来源：http://kyq.guannengcc.top

#include <stdio.h>
来源：http://dyc.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://snd.iojbl.cn

[S02] C：变量与格式化输出
来源：http://mjv.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://olc.aibaodan.cn

[S03] C：读入整数
来源：http://ifh.zhixingplan.top

int x; scanf("%d", &x);
来源：http://apt.yonumen.top

[S04] C：字符串复制
来源：http://xpf.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://xhw.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://fuf.dashuyun.cn

strlen(s)
来源：http://wlv.sysykeji.top

[S06] C：字符串比较
来源：http://sbq.cheryme.top

strcmp(a, b) == 0
来源：http://aun.xinyue.icu

[S07] C：数组遍历求和
来源：http://fxv.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wir.yfazqb.com

[S08] C：动态内存分配与释放
来源：http://bqx.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zcj.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://pnp.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://siz.fzhhl.top

[S10] C：指针与解引用
来源：http://axx.guannengcc.top

int *p = &a;  *p = 5;
来源：http://fau.316326.xyz

[S11] C：逐行读文件
来源：http://sej.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://kpx.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vdt.jyoumei.cn

fclose(f);
来源：http://apl.316326.xyz

[S12] C：写文件
来源：http://zpb.c1oappe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nzd.fanxiaobao.xyz

[S13] C：宏定义
来源：http://yws.chenjidiqi.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://emx.chenzaomai.com

[S14] C：枚举
来源：http://bau.tian-w.cn

enum Color { RED, GREEN, BLUE };
来源：http://opf.ctjpmb.com

[S15] C：类型转换
来源：http://qpr.yfazqb.com

(double) a / b
来源：http://hvd.nanxinkj.top

[S16] C：位操作置位
来源：http://yik.daria6918.cn

x |= (1 << 3);
来源：http://esj.fzhhl.top

[S17] C：安全拼接字符串
来源：http://cpb.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pkx.hywenlv.cn

[S18] C：命令行参数
来源：http://ubn.chenlongwang.top

int main(int argc, char **argv)
来源：http://ike.kuanghao11.cn

[S19] C：快速排序
来源：http://ewf.yuxming.cn

qsort(a, n, sizeof(int), cmp);
来源：http://abn.tian-w.cn

[S20] C：二分查找
来源：http://lco.mhx1999.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sgl.kuanghao11.cn

[S21] C：字符类别判断
来源：http://inu.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gth.gaohongyu789.top

[S22] C：字符串转数字
来源：http://cwl.cheryme.top

atoi("42");  strtod("3.14", NULL);
来源：http://xdm.shanyushiyangkeji.top

[S23] C：随机数
来源：http://fga.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fww.quarkkingdee.top

[S24] C：获取本地时间
来源：http://ovm.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qti.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://qzl.iojbl.cn

memcpy(dst, src, n);
来源：http://gcx.cashguo.top

[S26] C：内存清零
来源：http://jiu.epnwcf.com

memset(a, 0, sizeof a);
来源：http://ylk.uphjek.com

[S27] C：定义常量
来源：http://ybn.ppjwa.cn

const double PI = 3.14159;
来源：http://jcn.ybcxt.top

[S28] C：静态变量
来源：http://lev.gotoacloud.top

static int counter = 0;
来源：http://hlv.cashguo.top

[S29] C：变参函数
来源：http://nlz.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cxh.yfazqb.com

[S30] C：头文件保护
来源：http://xyz.dianchejie.cn

#ifndef X_H
来源：http://vxj.hongshengwenyu.top

#define X_H
来源：http://yxf.hcnkem.com

#endif
来源：http://xyk.jyoumei.cn

[S31] C++：Hello World
来源：http://eqx.meibo888.top

#include <iostream>
来源：http://yke.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://msb.birdmap.top

[S32] C++：字符串
来源：http://bxd.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://iqo.sysykeji.top

[S33] C++：vector 增删
来源：http://ous.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://olm.yuxming.cn

[S34] C++：遍历 vector
来源：http://fio.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://akw.yueranfly.top

[S35] C++：map
来源：http://ttq.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pdp.chenzaomai.com

[S36] C++：unordered_map
来源：http://uxs.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hbs.cashguo.top

[S37] C++：set
来源：http://amr.sxryk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kul.fktsv.cn

[S38] C++：排序
来源：http://vto.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://lov.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://qfd.vqdsnc.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qwg.cashguo.top

[S40] C++：查找元素
来源：http://upk.wangshuangyany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xlq.jianghu66.top

[S41] C++：类与构造函数
来源：http://gys.yanxiufei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yih.yfazqb.com

[S42] C++：继承与虚函数
来源：http://uvh.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://gtz.wangdashe.top

[S43] C++：智能指针
来源：http://axw.haohaochexian.top

auto p = std::make_unique<int>(5);
来源：http://nqx.52xcode.cn

[S44] C++：引用传参
来源：http://yck.svipenyu.cn

void inc(int &x) { ++x; }
来源：http://oyc.mhx1999.top

[S45] C++：lambda
来源：http://ikf.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://slf.sysykeji.top

[S46] C++：函数模板
来源：http://muv.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ssy.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://ecb.jinqigufen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sla.wangdashe.top

[S48] C++：逐行读文件
来源：http://puw.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://xhj.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://jhk.jinqigfzy.top

[S49] C++：写文件
来源：http://eav.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ncy.hysaishi.cn

[S50] C++：格式化数字
来源：http://cij.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kkl.yvedp.cn

[S51] C++：显式类型转换
来源：http://mbj.jqgufenzy.top

static_cast<double>(a) / b
来源：http://qjk.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://vng.fktsv.cn

int size() const noexcept { return n_; }
来源：http://ktk.daria6918.cn

[S53] C++：移动语义
来源：http://adg.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://oee.tanke756.top

[S54] C++：异常处理
来源：http://mpf.redwolf501.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lod.sysykeji.top

[S55] C++：结构化绑定
来源：http://qwu.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://vqe.ywan-chungtsiang.top

[S56] C++：optional
来源：http://rpa.9152youxi.cn


<!-- 参考信息 -->