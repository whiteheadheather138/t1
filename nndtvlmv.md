代发 wailian999

[Q84] 去除首尾空格
来源：http://veb.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://uqj.gzhubu.top

[Q85] 数值取整
来源：http://vys.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lqa.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://kef.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lim.hammf.cn

[Q87] JSON 字段做条件
来源：http://ajv.hywenlv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ibz.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://rel.jinyuanbaomall.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://boz.nanxinkj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qdc.hfpthk.cn

[Q89] 判断表是否存在
来源：http://rzq.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zwi.zhixingplan.top

[Q90] 生成序号列
来源：http://lgs.yuanzhike.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gxf.yueranfly.top

================================================================================
来源：http://wfg.svipenyu.cn

R. Bash 专题
来源：http://iad.hnqzz.top

================================================================================
来源：http://jqv.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://zqr.gotoacloud.top

#!/usr/bin/env bash
来源：http://ocd.nwbrower.top

set -euo pipefail
来源：http://glf.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://vpy.cashguo.top

name="Tom"; echo "$name"
来源：http://evx.epnwcf.com

[R03] 只读变量
来源：http://hvo.hfpthk.cn

readonly PI=3.14
来源：http://tfg.yangfankeji.com

[R04] 位置参数
来源：http://kvo.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sss.meibo888.top

[R05] 参数默认值
来源：http://zha.nanxuanxn.top

name="${1:-default}"
来源：http://zta.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://wgd.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dqf.vqdsnc.cn

[R07] if 判断文件
来源：http://urd.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gbq.tian-w.cn

[R08] 数值比较
来源：http://xtf.fengsongda.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rzi.zhiwuduotai.top

[R09] 字符串比较
来源：http://qtd.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xob.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://iqk.haohaochexian.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zvz.jqgufenzy.top

[R11] case 多分支
来源：http://asr.feifeiyinyue.top

case "$1" in
来源：http://fwd.haohaochexian.top

start) echo "启动" ;;
来源：http://khj.vqdsnc.cn

stop)  echo "停止" ;;
来源：http://pgk.uphjek.com

*)     echo "未知命令" ;;
来源：http://fhx.meibo888.top

esac
来源：http://zkp.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://who.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://kus.andypj.xyz

[R13] for 计数循环
来源：http://iih.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://umb.yj20258888.top

[R14] C 风格 for
来源：http://cvv.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gdl.yuxming.cn

[R15] while 逐行读文件
来源：http://gmx.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://isz.jianghu66.top

[R16] until 等待条件
来源：http://tzd.daxiang520.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ljl.shangyingyoupin.top

[R17] 数组定义与取值
来源：http://jht.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://omj.nanxuanxn.top

[R18] 遍历数组
来源：http://osl.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jbp.zhongyouzk.top

[R19] 数组长度
来源：http://nuk.aizwys.cn

echo "${#arr[@]}"
来源：http://azk.quarkkingdee.top

[R20] 关联数组（字典）
来源：http://woy.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lez.c1oappe.top

[R21] 字符串长度
来源：http://pxn.fengsongda.top

echo "${#s}"
来源：http://oyr.gaohongyu789.top

[R22] 截取子串
来源：http://qjk.guowangkeji.top

echo "${s:0:5}"
来源：http://rcm.xuetiantiany.cn

[R23] 字符串替换
来源：http://tow.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iyd.xinyue.icu

[R24] 大小写转换
来源：http://lfp.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://mlo.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://oat.chenzaomai.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://bph.ydjk.org.cn

[R26] 命令替换
来源：http://hhm.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://nzu.yuanzhike.top

[R27] 算术展开
来源：http://sda.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://qcr.52xcode.cn

[R28] 浮点运算
来源：http://kma.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://ice.ctjpmb.com

[R29] 定义函数
来源：http://zmo.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fcp.gogol.net.cn

[R30] 函数返回状态码
来源：http://csb.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://pij.chenlongwang.top

[R31] 局部变量
来源：http://mev.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://yfs.sufxvd.cn

[R32] 参数个数校验
来源：http://ion.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hjf.52xcode.cn

[R33] 捕获错误并提示行号
来源：http://lfz.ybcxt.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gam.feifeiyinyue.top

[R34] 退出时清理
来源：http://iqq.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://xck.ivvv.top

[R35] 后台执行并等待
来源：http://ohr.snrcjt.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ztf.nanxinkj.top

[R36] 并发执行多个任务
来源：http://pdu.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jil.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://wjc.chenlongwang.top

files=$(ls -1)
来源：http://mrt.xinyue.icu

[R38] 管道串联
来源：http://gtr.yuxming.cn

cat a.txt | grep -i error | wc -l
来源：http://fno.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://egy.zhoulong.xyz

cmd > out.log 2>&1
来源：http://nca.ctjpmb.com

[R40] 追加写日志
来源：http://rvc.aizwys.cn

echo "log" >> out.log
来源：http://gxk.xziqi.cn

[R41] 丢弃输出
来源：http://tie.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://zfl.hongshengwenyu.top

[R42] 输入重定向
来源：http://lyf.shzxlz.cn

wc -l < a.txt
来源：http://sfp.snrcjt.cn

[R43] 按名字查找文件
来源：http://hmw.birdmap.top

find . -name "*.log" -type f
来源：http://zff.birdmap.top

[R44] 按修改时间查找
来源：http://xly.zdbjq.cn

find . -mtime -7 -type f
来源：http://hlo.dashuyun.cn

[R45] 批量删除
来源：http://wke.zhengqikj.top

find . -name "*.tmp" -delete
来源：http://oul.andypj.xyz

[R46] 递归替换文件内容
来源：http://ure.bbcook.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nqv.yonumen.top

[R47] sed 单行替换
来源：http://elu.daxiang520.top

sed -i 's/foo/bar/g' a.txt
来源：http://xxs.yongpay.top

[R48] awk 取指定列
来源：http://bjc.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://xqb.gaohongyu789.top

[R49] awk 带条件
来源：http://vbe.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://egi.gotoacloud.top

[R50] awk 求和
来源：http://kiv.jqgfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://siv.yfazqb.com

[R51] 排序去重取前几
来源：http://rhx.xziqi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sie.hesvh.cn

[R52] 统计行数
来源：http://fnj.aizwys.cn

wc -l a.txt
来源：http://eif.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://nou.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pql.redwolf501.top

[R54] 比较两个文件
来源：http://oyc.chenjidiqi.icu

diff a.txt b.txt
来源：http://hub.cdnleiting.top

[R55] 压缩与解压
来源：http://bew.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jal.jianghu66.top

[R56] 远程拷贝
来源：http://baj.shanyushiyangtech.top

scp file user@host:/path/
来源：http://zas.zycfv.cn

[R57] 远程执行命令
来源：http://lmx.cqqwz.cn

ssh user@host 'uptime'
来源：http://eyf.gzhubu.top

[R58] 下载文件
来源：http://stz.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://npd.chenlongwang.top

[R59] 发 POST JSON
来源：http://ijg.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sok.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://vgw.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sdv.shzxlz.cn

[R61] 磁盘占用
来源：http://ljy.xinyue.icu

df -h;  du -sh *
来源：http://vyp.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://wba.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://vnd.yanxiufei.cn

[R63] 内存与进程
来源：http://mvz.ctjpmb.com

free -h;  ps aux | grep nginx
来源：http://bcs.nanxuanxn.top

[R64] 结束进程
来源：http://wdd.redwolf501.top

kill -9 $(pgrep -f app.py)
来源：http://klv.yj20258.top

[R65] 查看端口占用
来源：http://iqv.cashguo.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cap.zycfv.cn

[R66] 定时任务
来源：http://ykq.xuanzx.com

crontab -e;  crontab -l
来源：http://lom.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://hrm.zhiwuduotai.top

openssl rand -hex 16
来源：http://hvp.zhoulong.xyz

[R68] 计算文件校验值
来源：http://ojo.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jqz.cashguo.top

[R69] 生成随机密码
来源：http://kzh.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://oai.haohaochexian.top

[R70] 时间戳与互转
来源：http://qaz.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://xlz.ehwqpu.com

[R71] 日期格式化
来源：http://wox.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mij.jlsjyb.cn

[R72] 等待端口就绪
来源：http://qlz.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://sds.yj202588.top

[R73] 分割大日志
来源：http://noc.tianlin.xyz

split -l 1000 big.log part_
来源：http://tsy.pengpengdd.cyou

[R74] 批量重命名
来源：http://xqz.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gph.9152youxi.cn

[R75] 导出环境变量
来源：http://csi.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://ftm.pengpengdd.cyou

[R76] 使用临时文件
来源：http://brc.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jpz.jiagoushi.top

[R77] 读取用户输入
来源：http://bsk.cucudq.cn

read -rp "请输入: " ans
来源：http://qrs.yonumen.top

[R78] 交互式菜单
来源：http://nsx.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qhs.gotoacloud.top

[R79] 解析命令行选项
来源：http://ebq.nanxinkj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wry.havefunace.top

[R80] 查看脚本执行耗时
来源：http://bwh.xuanzx.com

time ./run.sh
来源：http://faj.hammf.cn

================================================================================
来源：http://jkh.xuetiantiany.cn

S. C / C++ 专题
来源：http://iwl.daria6918.cn

================================================================================
来源：http://dua.tarul.cn

[S01] C：Hello World
来源：http://syd.andypj.xyz

#include <stdio.h>
来源：http://eod.zycfv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rmo.xziqi.cn

[S02] C：变量与格式化输出
来源：http://rgm.jqgufenzy.top

int a = 10; printf("%d\n", a);
来源：http://xai.nanxinkj.top

[S03] C：读入整数
来源：http://nhd.bbcook.cn

int x; scanf("%d", &x);
来源：http://eyw.chenzaomai.com

[S04] C：字符串复制
来源：http://anv.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lgm.pengpengdd.cyou

[S05] C：字符串长度
来源：http://vco.fanxiaobao.xyz

strlen(s)
来源：http://kag.bjfxy.top

[S06] C：字符串比较
来源：http://nit.hysaishi.cn

strcmp(a, b) == 0
来源：http://qbu.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://qbt.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://scx.tianlin.xyz

[S08] C：动态内存分配与释放
来源：http://wdv.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yxl.zhoulong.xyz

[S09] C：结构体定义与初始化
来源：http://fnl.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pvg.yvedp.cn

[S10] C：指针与解引用
来源：http://dxo.ydzc1.top

int *p = &a;  *p = 5;
来源：http://cgd.yuxming.cn

[S11] C：逐行读文件
来源：http://qgd.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://nhy.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://eey.birdmap.top

fclose(f);
来源：http://hjq.pengpengdd.cyou

[S12] C：写文件
来源：http://yyh.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bzf.jiagoushi.top

[S13] C：宏定义
来源：http://zkw.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://emq.sysykeji.top

[S14] C：枚举
来源：http://vgf.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://twj.shuidangran.top

[S15] C：类型转换
来源：http://btc.gzhubu.top

(double) a / b
来源：http://ocs.redwolf501.top

[S16] C：位操作置位
来源：http://tck.gogol.net.cn

x |= (1 << 3);
来源：http://hox.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://lgr.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nii.bjfxy.top

[S18] C：命令行参数
来源：http://osl.cqqwz.cn

int main(int argc, char **argv)
来源：http://qtj.andypj.xyz

[S19] C：快速排序
来源：http://oej.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kwh.cashguo.top

[S20] C：二分查找
来源：http://hlk.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eiw.ppjwa.cn

[S21] C：字符类别判断
来源：http://fgg.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://khx.zhengqikj.top

[S22] C：字符串转数字
来源：http://jrr.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wua.xuetiantiany.cn

[S23] C：随机数
来源：http://ikx.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://bnh.kuanghao11.cn

[S24] C：获取本地时间
来源：http://ynd.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zcj.cdnleiting.top

[S25] C：内存拷贝
来源：http://sek.daxiang520.top

memcpy(dst, src, n);
来源：http://xmo.vehdjk.com

[S26] C：内存清零
来源：http://lvb.hcnkem.com

memset(a, 0, sizeof a);
来源：http://swd.quarkkingdee.top

[S27] C：定义常量
来源：http://rpz.zycfv.cn

const double PI = 3.14159;
来源：http://pun.chenzaomai.com

[S28] C：静态变量
来源：http://tso.bbcook.cn

static int counter = 0;
来源：http://eho.vehdjk.com

[S29] C：变参函数
来源：http://zez.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://whc.yj202588.top

[S30] C：头文件保护
来源：http://qym.ehwqpu.com

#ifndef X_H
来源：http://bfx.nwbrower.top

#define X_H
来源：http://ufn.hongshengwenyu.top

#endif
来源：http://kgt.ybcxt.top

[S31] C++：Hello World
来源：http://bzy.yj202588.top

#include <iostream>
来源：http://afl.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://hfz.sweek.top

[S32] C++：字符串
来源：http://ukf.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://awo.mhx1999.top

[S33] C++：vector 增删
来源：http://vhr.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zkt.ctjpmb.com

[S34] C++：遍历 vector
来源：http://aom.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://sjd.ydjk.org.cn

[S35] C++：map
来源：http://vrm.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nbq.bbcook.cn

[S36] C++：unordered_map
来源：http://ijj.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lyu.hfpthk.cn

[S37] C++：set
来源：http://pob.yuxming.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qde.sxryk.cn

[S38] C++：排序
来源：http://yff.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://lji.zhoulong.xyz

[S39] C++：自定义比较器排序
来源：http://kht.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cvn.xylfe.cn

[S40] C++：查找元素
来源：http://zpl.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cfr.bbcook.cn

[S41] C++：类与构造函数
来源：http://ufc.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tuj.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://kfp.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://dhr.chenzaomai.com

[S43] C++：智能指针
来源：http://tdz.fktsv.cn

auto p = std::make_unique<int>(5);
来源：http://ebr.aibaodan.cn

[S44] C++：引用传参
来源：http://kgr.yongpay.top

void inc(int &x) { ++x; }
来源：http://wrv.iojbl.cn

[S45] C++：lambda
来源：http://lcp.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://miq.pycfn.com

[S46] C++：函数模板
来源：http://vyn.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zwq.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://fgt.cashguo.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rcr.aibaodan.cn

[S48] C++：逐行读文件
来源：http://ikv.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://ims.xinyue.icu

while (std::getline(in, line)) { }
来源：http://qga.kuanghao11.cn

[S49] C++：写文件
来源：http://fcl.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tuc.jinqigufen.top

[S50] C++：格式化数字
来源：http://yzc.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xrd.ppjwa.cn

[S51] C++：显式类型转换
来源：http://bvw.nwbrower.top

static_cast<double>(a) / b
来源：http://jju.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://ceu.jqgfzy.top

int size() const noexcept { return n_; }
来源：http://atf.gzhubu.top

[S53] C++：移动语义
来源：http://ark.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://axc.cheryme.top

[S54] C++：异常处理
来源：http://zdg.hysaishi.cn


<!-- 参考信息 -->