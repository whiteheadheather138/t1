代发 wailian999

[Q80] 字符串截取
来源：http://fol.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uzf.tianlin.xyz

[Q81] 字符串替换
来源：http://slu.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cci.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://and.yj20258888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ycr.feifeiyinyue.top

[Q83] 大小写转换
来源：http://xvl.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://izy.redwolf501.top

[Q84] 去除首尾空格
来源：http://ydr.andypj.xyz

SELECT TRIM(name) FROM users;
来源：http://yet.ivvv.top

[Q85] 数值取整
来源：http://fvl.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hoo.tanke756.top

[Q86] 读取 JSON 字段
来源：http://rzh.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hci.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://twx.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yza.cheryme.top

[Q88] 行转列（条件聚合）
来源：http://xep.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://stk.zycfv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jjb.xuanzx.com

[Q89] 判断表是否存在
来源：http://jje.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://euy.epnwcf.com

[Q90] 生成序号列
来源：http://ahf.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nnp.chenzaomai.com

================================================================================
来源：http://wlz.daria6918.cn

R. Bash 专题
来源：http://gqa.guowangkeji.top

================================================================================
来源：http://acm.tian-w.cn

[R01] shebang 与严格模式
来源：http://piu.jyoumei.cn

#!/usr/bin/env bash
来源：http://hdq.aizwys.cn

set -euo pipefail
来源：http://uql.zdbjq.cn

[R02] 变量赋值与使用
来源：http://faz.ybcxt.top

name="Tom"; echo "$name"
来源：http://exr.hesvh.cn

[R03] 只读变量
来源：http://sqp.ehwqpu.com

readonly PI=3.14
来源：http://oyy.fengsongda.top

[R04] 位置参数
来源：http://foq.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cha.hysaishi.cn

[R05] 参数默认值
来源：http://pgx.ctjpmb.com

name="${1:-default}"
来源：http://hps.bjfxy.top

[R06] 判断命令是否存在
来源：http://cel.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://prl.yueranfly.top

[R07] if 判断文件
来源：http://rvm.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xkh.zdbjq.cn

[R08] 数值比较
来源：http://ffq.hammf.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hic.iojbl.cn

[R09] 字符串比较
来源：http://xej.sjlbkw.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xry.fzhhl.top

[R10] 正则匹配
来源：http://lwt.jiagoushi.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ofv.yanxiufei.cn

[R11] case 多分支
来源：http://teq.mhx1999.top

case "$1" in
来源：http://bcp.jianghu66.top

start) echo "启动" ;;
来源：http://szq.epnwcf.com

stop)  echo "停止" ;;
来源：http://iwh.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://sbw.hammf.cn

esac
来源：http://fgh.snrcjt.cn

[R12] for 遍历文件
来源：http://hwh.epnwcf.com

for f in *.txt; do echo "$f"; done
来源：http://snf.zhongyouzk.top

[R13] for 计数循环
来源：http://goz.hcnkem.com

for i in {1..10}; do echo "$i"; done
来源：http://mis.bbcook.cn

[R14] C 风格 for
来源：http://wlp.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gtt.sufxvd.cn

[R15] while 逐行读文件
来源：http://pln.snrcjt.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://auv.nwbrower.top

[R16] until 等待条件
来源：http://qav.haohaochexian.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uxf.ywan-chungtsiang.top

[R17] 数组定义与取值
来源：http://uvw.zhixingplan.top

arr=(a b c); echo "${arr[0]}"
来源：http://job.fehbvm.com

[R18] 遍历数组
来源：http://ltb.cdnleiting.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ypk.yongpay.top

[R19] 数组长度
来源：http://efk.sweek.top

echo "${#arr[@]}"
来源：http://amj.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://uzh.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://syv.yj20258888.top

[R21] 字符串长度
来源：http://kei.c1oappe.top

echo "${#s}"
来源：http://bwq.hammf.cn

[R22] 截取子串
来源：http://scy.zdqjudy.top

echo "${s:0:5}"
来源：http://tco.zdqjudy.top

[R23] 字符串替换
来源：http://uml.jinghuilouyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xey.wangdashe.top

[R24] 大小写转换
来源：http://bze.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ctp.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://uwm.jyoumei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bcd.sufxvd.cn

[R26] 命令替换
来源：http://qzj.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://lfn.fzhhl.top

[R27] 算术展开
来源：http://egb.hysaishi.cn

echo $((1 + 2 * 3))
来源：http://wqr.jqgfzy.top

[R28] 浮点运算
来源：http://bum.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://qet.zdbjq.cn

[R29] 定义函数
来源：http://qtp.zhengqikj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yre.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://mfk.ydzc1.top

f() { return 0; }; f || echo "失败了"
来源：http://ufk.fanxiaobao.xyz

[R31] 局部变量
来源：http://xqt.yvedp.cn

f() { local x=1; echo "$x"; }
来源：http://omm.shzxlz.cn

[R32] 参数个数校验
来源：http://ukw.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lmo.hywenlv.cn

[R33] 捕获错误并提示行号
来源：http://uly.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://snv.dashuyun.cn

[R34] 退出时清理
来源：http://wce.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cjh.guowangkeji.top

[R35] 后台执行并等待
来源：http://unm.hcnkem.com

sleep 5 & pid=$!; wait "$pid"
来源：http://sxx.birdmap.top

[R36] 并发执行多个任务
来源：http://elj.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kqc.yuxming.cn

[R37] 把输出赋给变量
来源：http://ilg.shzxlz.cn

files=$(ls -1)
来源：http://ttd.shuidangran.top

[R38] 管道串联
来源：http://sls.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://nuy.yj20258.top

[R39] 重定向标准输出与错误
来源：http://nba.hfpthk.cn

cmd > out.log 2>&1
来源：http://cqp.yuanzhike.top

[R40] 追加写日志
来源：http://jxg.hongshengwenyu.top

echo "log" >> out.log
来源：http://bpn.tianlin.xyz

[R41] 丢弃输出
来源：http://ntj.c1oappe.top

cmd >/dev/null 2>&1
来源：http://and.zhoulong.xyz

[R42] 输入重定向
来源：http://bia.ehwqpu.com

wc -l < a.txt
来源：http://igd.zhoulong.xyz

[R43] 按名字查找文件
来源：http://lvs.52xcode.cn

find . -name "*.log" -type f
来源：http://hni.cdnleiting.top

[R44] 按修改时间查找
来源：http://dwy.wangdashe.top

find . -mtime -7 -type f
来源：http://iiw.xinyue.icu

[R45] 批量删除
来源：http://dfc.smart0.xyz

find . -name "*.tmp" -delete
来源：http://aby.jinghuilouyu.cn

[R46] 递归替换文件内容
来源：http://jxn.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qbf.tarul.cn

[R47] sed 单行替换
来源：http://sga.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://djr.dashuyun.cn

[R48] awk 取指定列
来源：http://pfb.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://sti.wangshuangyany.cn

[R49] awk 带条件
来源：http://mii.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oha.wangdashe.top

[R50] awk 求和
来源：http://yqt.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ocl.bjfxy.top

[R51] 排序去重取前几
来源：http://njm.zdbjq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kho.yj20258888.top

[R52] 统计行数
来源：http://zws.zhongyouzk.top

wc -l a.txt
来源：http://xax.jianghu66.top

[R53] 查看文件头与实时尾
来源：http://vmj.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dhi.dianchejie.cn

[R54] 比较两个文件
来源：http://ytd.fktsv.cn

diff a.txt b.txt
来源：http://sfb.daxiang520.top

[R55] 压缩与解压
来源：http://cqw.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jhi.shangyingyoupin.top

[R56] 远程拷贝
来源：http://qob.pycfn.com

scp file user@host:/path/
来源：http://gwe.fktsv.cn

[R57] 远程执行命令
来源：http://ina.birdmap.top

ssh user@host 'uptime'
来源：http://iqc.0kj1m.cn

[R58] 下载文件
来源：http://kie.zhiwuduotai.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://giq.sjlbkw.cn

[R59] 发 POST JSON
来源：http://qla.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://beo.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://pgq.tian-w.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qko.guowangkeji.top

[R61] 磁盘占用
来源：http://ffe.cashguo.top

df -h;  du -sh *
来源：http://kvo.jianghu66.top

[R62] 找最占空间的文件
来源：http://zvp.cdnleiting.top

du -ah . | sort -rh | head -10
来源：http://hlz.hammf.cn

[R63] 内存与进程
来源：http://ctx.ivvv.top

free -h;  ps aux | grep nginx
来源：http://enq.zhiwuduotai.top

[R64] 结束进程
来源：http://zds.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://lbh.ivvv.top

[R65] 查看端口占用
来源：http://obe.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fpb.cdnleiting.top

[R66] 定时任务
来源：http://les.sweek.top

crontab -e;  crontab -l
来源：http://vij.zycfv.cn

[R67] 生成随机十六进制串
来源：http://gkc.quarkkingdee.top

openssl rand -hex 16
来源：http://hcs.yfazqb.com

[R68] 计算文件校验值
来源：http://mty.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://xjt.nanxinkj.top

[R69] 生成随机密码
来源：http://mee.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://xlj.dashuyun.cn

[R70] 时间戳与互转
来源：http://iuq.dianchejie.cn

date +%s;  date -d @1700000000
来源：http://bpp.yfazqb.com

[R71] 日期格式化
来源：http://quk.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rde.zdqjudy.top

[R72] 等待端口就绪
来源：http://hoa.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://zpg.andypj.xyz

[R73] 分割大日志
来源：http://mdu.xinyue.icu

split -l 1000 big.log part_
来源：http://yup.dianchejie.cn

[R74] 批量重命名
来源：http://nks.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xvk.nanxinkj.top

[R75] 导出环境变量
来源：http://ynd.vqdsnc.cn

export PATH="$HOME/bin:$PATH"
来源：http://nnw.xylfe.cn

[R76] 使用临时文件
来源：http://nyg.hywenlv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sip.dianchejie.cn

[R77] 读取用户输入
来源：http://fjg.0kj1m.cn

read -rp "请输入: " ans
来源：http://fvk.andypj.xyz

[R78] 交互式菜单
来源：http://rni.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gvm.yangfankeji.com

[R79] 解析命令行选项
来源：http://ybr.c1oappe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vbg.yonumen.top

[R80] 查看脚本执行耗时
来源：http://rab.cashguo.top

time ./run.sh
来源：http://dzy.gaohongyu789.top

================================================================================
来源：http://dqo.jianghu66.top

S. C / C++ 专题
来源：http://mjt.gzhubu.top

================================================================================
来源：http://esv.hammf.cn

[S01] C：Hello World
来源：http://jjc.dashuyun.cn

#include <stdio.h>
来源：http://ysu.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jrg.hnxiangtu.top

[S02] C：变量与格式化输出
来源：http://xye.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://fpg.nanxuanxn.top

[S03] C：读入整数
来源：http://jlf.chenzaomai.com

int x; scanf("%d", &x);
来源：http://obj.jiagoushi.top

[S04] C：字符串复制
来源：http://mnb.hnqzz.top

char dst[32]; strcpy(dst, "hi");
来源：http://mtf.bjfxy.top

[S05] C：字符串长度
来源：http://kgf.9152youxi.cn

strlen(s)
来源：http://gbe.uphjek.com

[S06] C：字符串比较
来源：http://fwj.shuidangran.top

strcmp(a, b) == 0
来源：http://cvz.gogol.net.cn

[S07] C：数组遍历求和
来源：http://lpx.fanxiaobao.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cxa.yj202588.top

[S08] C：动态内存分配与释放
来源：http://huv.jqgufenzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://muv.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://wfk.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cxw.zdqjudy.top

[S10] C：指针与解引用
来源：http://emx.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://wkl.nwbrower.top

[S11] C：逐行读文件
来源：http://gql.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://tsm.zycfv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://whw.cdnleiting.top

fclose(f);
来源：http://baa.nanxinkj.top

[S12] C：写文件
来源：http://bhc.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oyo.zhijiandao.cn

[S13] C：宏定义
来源：http://ulc.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://das.smart0.xyz

[S14] C：枚举
来源：http://dbs.smart0.xyz

enum Color { RED, GREEN, BLUE };
来源：http://umz.tanke756.top

[S15] C：类型转换
来源：http://ade.ivvv.top

(double) a / b
来源：http://myn.jyoumei.cn

[S16] C：位操作置位
来源：http://ynl.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://rxh.cucudq.cn

[S17] C：安全拼接字符串
来源：http://qzv.yj202588.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://noe.jinghuilouyu.cn

[S18] C：命令行参数
来源：http://ufz.hnqzz.top

int main(int argc, char **argv)
来源：http://dpy.yfazqb.com

[S19] C：快速排序
来源：http://web.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://hfv.svipenyu.cn

[S20] C：二分查找
来源：http://haf.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ups.hammf.cn

[S21] C：字符类别判断
来源：http://fan.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nys.pycfn.com

[S22] C：字符串转数字
来源：http://wzl.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://wau.kuanghao11.cn

[S23] C：随机数
来源：http://bjd.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ogs.vehdjk.com

[S24] C：获取本地时间
来源：http://opv.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://agn.ehwqpu.com

[S25] C：内存拷贝
来源：http://yjc.zhengqikj.top

memcpy(dst, src, n);
来源：http://xhr.sufxvd.cn

[S26] C：内存清零
来源：http://ezz.mhx1999.top

memset(a, 0, sizeof a);
来源：http://jlp.jqgfzy.top

[S27] C：定义常量
来源：http://zmo.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://hrz.yvedp.cn

[S28] C：静态变量
来源：http://gqx.shangyingyoupin.top

static int counter = 0;
来源：http://nxz.cqqwz.cn

[S29] C：变参函数
来源：http://tyk.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xby.guannengcc.top

[S30] C：头文件保护
来源：http://mli.jlsjyb.cn

#ifndef X_H
来源：http://bxo.svipenyu.cn

#define X_H
来源：http://ofs.hongshengwenyu.top

#endif
来源：http://vwg.kuanghao11.cn

[S31] C++：Hello World
来源：http://gtp.sysykeji.top

#include <iostream>
来源：http://hxg.fanxiaobao.xyz

int main() { std::cout << "Hello\n"; }
来源：http://cdw.dianchejie.cn

[S32] C++：字符串
来源：http://zrj.birdmap.top

std::string s = "hi";  s += "!";
来源：http://xum.hywenlv.cn

[S33] C++：vector 增删
来源：http://fmf.fzhhl.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lch.ybcxt.top

[S34] C++：遍历 vector
来源：http://lsy.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://kzd.hongshengwenyu.top

[S35] C++：map
来源：http://xbu.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mfk.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://twa.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://acs.xziqi.cn

[S37] C++：set
来源：http://pbs.snrcjt.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vhk.vqdsnc.cn

[S38] C++：排序
来源：http://zxg.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://krr.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://wyj.ydzc1.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xxj.wangdashe.top

[S40] C++：查找元素
来源：http://dea.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nsn.zdbjq.cn

[S41] C++：类与构造函数
来源：http://xts.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ttr.fengsongda.top

[S42] C++：继承与虚函数
来源：http://ejs.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://smd.316326.xyz

[S43] C++：智能指针
来源：http://bvn.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://gbb.zhiwuduotai.top

[S44] C++：引用传参
来源：http://bxh.zhoulong.xyz

void inc(int &x) { ++x; }
来源：http://bkj.zdqjudy.top

[S45] C++：lambda
来源：http://rbm.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ibo.dashuyun.cn

[S46] C++：函数模板
来源：http://xzm.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lbg.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://pqk.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yft.nanxinkj.top

[S48] C++：逐行读文件
来源：http://rsd.sysykeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://mgk.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://ytx.zhoulong.xyz

[S49] C++：写文件
来源：http://wzt.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://udm.havefunace.top

[S50] C++：格式化数字
来源：http://ejf.vqdsnc.cn


<!-- 参考信息 -->