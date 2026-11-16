代发 wailian999

[Q78] 当前时间
来源：http://nwp.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ltn.chenlongwang.top

[Q79] 字符串拼接
来源：http://uul.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ywe.ctjpmb.com

[Q80] 字符串截取
来源：http://nyx.dashuyun.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gld.hnqzz.top

[Q81] 字符串替换
来源：http://ges.guowangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vse.yvedp.cn

[Q82] 字符长度与字节长度
来源：http://bvu.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wiq.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://rwx.nwbrower.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nmm.jianghu66.top

[Q84] 去除首尾空格
来源：http://rov.yongpay.top

SELECT TRIM(name) FROM users;
来源：http://tws.shangyingyoupin.top

[Q85] 数值取整
来源：http://khl.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mqj.zhongyouzk.top

[Q86] 读取 JSON 字段
来源：http://siv.jlsjyb.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qgh.yonumen.top

[Q87] JSON 字段做条件
来源：http://ziy.chenjidiqi.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yqs.kuanghao11.cn

[Q88] 行转列（条件聚合）
来源：http://zqi.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wqy.jiagoushi.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gcf.ctjpmb.com

[Q89] 判断表是否存在
来源：http://krp.yangfankeji.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uzb.nwbrower.top

[Q90] 生成序号列
来源：http://rkq.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qas.chenlongwang.top

================================================================================
来源：http://mre.yj202588.top

R. Bash 专题
来源：http://zvn.cucudq.cn

================================================================================
来源：http://mzm.cqqwz.cn

[R01] shebang 与严格模式
来源：http://xpp.guowangkeji.top

#!/usr/bin/env bash
来源：http://stz.cqqwz.cn

set -euo pipefail
来源：http://qjw.ehwqpu.com

[R02] 变量赋值与使用
来源：http://gpj.gzhubu.top

name="Tom"; echo "$name"
来源：http://iit.yvedp.cn

[R03] 只读变量
来源：http://jtf.cashguo.top

readonly PI=3.14
来源：http://ixn.zdqjudy.top

[R04] 位置参数
来源：http://wfb.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xvq.quarkkingdee.top

[R05] 参数默认值
来源：http://nea.9152youxi.cn

name="${1:-default}"
来源：http://asv.pycfn.com

[R06] 判断命令是否存在
来源：http://ozr.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xxg.xinyue.icu

[R07] if 判断文件
来源：http://cxp.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ykh.haohaochexian.top

[R08] 数值比较
来源：http://jum.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ukd.316326.xyz

[R09] 字符串比较
来源：http://hoc.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fox.sufxvd.cn

[R10] 正则匹配
来源：http://pqd.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oqw.epnwcf.com

[R11] case 多分支
来源：http://tfc.zhoulong.xyz

case "$1" in
来源：http://avv.yfazqb.com

start) echo "启动" ;;
来源：http://abk.birdmap.top

stop)  echo "停止" ;;
来源：http://sbg.jianghu66.top

*)     echo "未知命令" ;;
来源：http://bls.jqgufenzy.top

esac
来源：http://hia.ivvv.top

[R12] for 遍历文件
来源：http://cwu.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://dbe.yanxiufei.cn

[R13] for 计数循环
来源：http://fut.guannengcc.top

for i in {1..10}; do echo "$i"; done
来源：http://uge.hammf.cn

[R14] C 风格 for
来源：http://kcg.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://skc.hysaishi.cn

[R15] while 逐行读文件
来源：http://udf.9152youxi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vmm.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://mzc.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://htf.zhoulong.xyz

[R17] 数组定义与取值
来源：http://bwt.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://jmx.birdmap.top

[R18] 遍历数组
来源：http://ptq.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://icn.wangdashe.top

[R19] 数组长度
来源：http://qod.cucudq.cn

echo "${#arr[@]}"
来源：http://pey.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://unq.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oxd.smart0.xyz

[R21] 字符串长度
来源：http://xkm.fengsongda.top

echo "${#s}"
来源：http://lrn.xingfuxueyuan.xyz

[R22] 截取子串
来源：http://vae.c1oappe.top

echo "${s:0:5}"
来源：http://zwn.jqgufenzy.top

[R23] 字符串替换
来源：http://ngl.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aqb.smart0.xyz

[R24] 大小写转换
来源：http://tfb.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lim.hcnkem.com

[R25] 去后缀 / 去前缀
来源：http://knh.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wie.quarkkingdee.top

[R26] 命令替换
来源：http://eac.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://qfr.xziqi.cn

[R27] 算术展开
来源：http://dqu.xziqi.cn

echo $((1 + 2 * 3))
来源：http://ecj.snrcjt.cn

[R28] 浮点运算
来源：http://wkn.hesvh.cn

echo "scale=2; 10/3" | bc
来源：http://aia.316326.xyz

[R29] 定义函数
来源：http://lgd.fktsv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qhl.jianghu66.top

[R30] 函数返回状态码
来源：http://rxr.ppjwa.cn

f() { return 0; }; f || echo "失败了"
来源：http://jna.xziqi.cn

[R31] 局部变量
来源：http://gbe.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://baz.aizwys.cn

[R32] 参数个数校验
来源：http://vgw.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://apo.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://lsu.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ytn.yvedp.cn

[R34] 退出时清理
来源：http://ujr.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://hie.zhoulong.xyz

[R35] 后台执行并等待
来源：http://bon.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ham.zdbjq.cn

[R36] 并发执行多个任务
来源：http://lph.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hnd.fengsongda.top

[R37] 把输出赋给变量
来源：http://xth.hnqzz.top

files=$(ls -1)
来源：http://dev.ydjk.org.cn

[R38] 管道串联
来源：http://acq.gzhubu.top

cat a.txt | grep -i error | wc -l
来源：http://owd.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://sfs.fzhhl.top

cmd > out.log 2>&1
来源：http://kit.xylfe.cn

[R40] 追加写日志
来源：http://awy.jlsjyb.cn

echo "log" >> out.log
来源：http://zjy.zhijiandao.cn

[R41] 丢弃输出
来源：http://xje.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://gci.smart0.xyz

[R42] 输入重定向
来源：http://vbe.birdmap.top

wc -l < a.txt
来源：http://php.sweek.top

[R43] 按名字查找文件
来源：http://nhl.yuanzhike.top

find . -name "*.log" -type f
来源：http://vil.chenlongwang.top

[R44] 按修改时间查找
来源：http://dky.zhixingplan.top

find . -mtime -7 -type f
来源：http://kjz.pycfn.com

[R45] 批量删除
来源：http://zmk.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://ogq.smart0.xyz

[R46] 递归替换文件内容
来源：http://yue.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cny.hysaishi.cn

[R47] sed 单行替换
来源：http://enl.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://qng.chenjidiqi.icu

[R48] awk 取指定列
来源：http://mut.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://fyf.tanke756.top

[R49] awk 带条件
来源：http://edz.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xiu.epnwcf.com

[R50] awk 求和
来源：http://mxx.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://otz.yuanzhike.top

[R51] 排序去重取前几
来源：http://uth.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tfu.daria6918.cn

[R52] 统计行数
来源：http://ond.meibo888.top

wc -l a.txt
来源：http://qqh.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://vni.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qmk.yueranfly.top

[R54] 比较两个文件
来源：http://gpg.bjfxy.top

diff a.txt b.txt
来源：http://nio.sysykeji.top

[R55] 压缩与解压
来源：http://ovy.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dyk.andypj.xyz

[R56] 远程拷贝
来源：http://mng.ehwqpu.com

scp file user@host:/path/
来源：http://uep.tarul.cn

[R57] 远程执行命令
来源：http://dog.yangfankeji.com

ssh user@host 'uptime'
来源：http://ucj.yongpay.top

[R58] 下载文件
来源：http://ijf.vehdjk.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://csi.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://oxh.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ulm.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://unw.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ayo.jqgufenzy.top

[R61] 磁盘占用
来源：http://kuc.ydjk.org.cn

df -h;  du -sh *
来源：http://iou.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://gqi.ydjk.org.cn

du -ah . | sort -rh | head -10
来源：http://zpp.redwolf501.top

[R63] 内存与进程
来源：http://hzo.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://lua.ctjpmb.com

[R64] 结束进程
来源：http://itq.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://ayf.pengpengdd.cyou

[R65] 查看端口占用
来源：http://ysd.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aah.jiagoushi.top

[R66] 定时任务
来源：http://slh.shanyushiyangtech.top

crontab -e;  crontab -l
来源：http://cas.mhx1999.top

[R67] 生成随机十六进制串
来源：http://fpq.zdbjq.cn

openssl rand -hex 16
来源：http://cay.yueranfly.top

[R68] 计算文件校验值
来源：http://rjj.zhiwuduotai.top

sha256sum a.txt;  md5sum a.txt
来源：http://hvk.mhx1999.top

[R69] 生成随机密码
来源：http://jmk.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://fkh.ydjk.org.cn

[R70] 时间戳与互转
来源：http://xal.hongshengwenyu.top

date +%s;  date -d @1700000000
来源：http://lyj.sysykeji.top

[R71] 日期格式化
来源：http://gkf.shangyingyoupin.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xug.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://mte.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://szn.xuetiantiany.cn

[R73] 分割大日志
来源：http://bel.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://rwl.snrcjt.cn

[R74] 批量重命名
来源：http://vdb.tianlin.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iqp.pycfn.com

[R75] 导出环境变量
来源：http://wfe.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://sqk.cdnleiting.top

[R76] 使用临时文件
来源：http://bsp.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nwo.tarul.cn

[R77] 读取用户输入
来源：http://gmi.yfazqb.com

read -rp "请输入: " ans
来源：http://imu.gogol.net.cn

[R78] 交互式菜单
来源：http://lkn.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fef.dashuyun.cn

[R79] 解析命令行选项
来源：http://geu.gogol.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rkr.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://uop.haohaochexian.top

time ./run.sh
来源：http://krn.yj20258.top

================================================================================
来源：http://unu.gaohongyu789.top

S. C / C++ 专题
来源：http://aqi.hammf.cn

================================================================================
来源：http://ubm.iojbl.cn

[S01] C：Hello World
来源：http://szz.yonumen.top

#include <stdio.h>
来源：http://ged.xinyue.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://dji.birdmap.top

[S02] C：变量与格式化输出
来源：http://ddy.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://dnr.nwbrower.top

[S03] C：读入整数
来源：http://tpk.yfazqb.com

int x; scanf("%d", &x);
来源：http://xld.dianchejie.cn

[S04] C：字符串复制
来源：http://puh.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://bkl.epnwcf.com

[S05] C：字符串长度
来源：http://kme.jiagoushi.top

strlen(s)
来源：http://txk.zdqjudy.top

[S06] C：字符串比较
来源：http://ygn.ppjwa.cn

strcmp(a, b) == 0
来源：http://mhc.yj202588.top

[S07] C：数组遍历求和
来源：http://kei.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pea.pycfn.com

[S08] C：动态内存分配与释放
来源：http://naz.gotoacloud.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hyb.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://tny.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mxv.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://htc.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://ebv.hnxiangtu.top

[S11] C：逐行读文件
来源：http://hhc.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://egd.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zep.redwolf501.top

fclose(f);
来源：http://ooa.zhaomingkeji.xyz

[S12] C：写文件
来源：http://xdo.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aha.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://lqn.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jdx.yj202588.top

[S14] C：枚举
来源：http://xzx.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://hqd.yangfankeji.com

[S15] C：类型转换
来源：http://ira.jqgfzy.top

(double) a / b
来源：http://iar.zycfv.cn

[S16] C：位操作置位
来源：http://yrv.jiagoushi.top

x |= (1 << 3);
来源：http://qbx.birdmap.top

[S17] C：安全拼接字符串
来源：http://ara.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kse.fzhhl.top

[S18] C：命令行参数
来源：http://kjx.yanxiufei.cn

int main(int argc, char **argv)
来源：http://eks.chenjidiqi.icu

[S19] C：快速排序
来源：http://xzc.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://lqb.yuanzhike.top

[S20] C：二分查找
来源：http://dzd.meibo888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ibw.yvedp.cn

[S21] C：字符类别判断
来源：http://vmj.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jyg.nanxinkj.top

[S22] C：字符串转数字
来源：http://vuw.hnxiangtu.top

atoi("42");  strtod("3.14", NULL);
来源：http://jet.dashuyun.cn

[S23] C：随机数
来源：http://yjs.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zyw.sufxvd.cn

[S24] C：获取本地时间
来源：http://tab.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nrg.shanyushiyangkeji.top

[S25] C：内存拷贝
来源：http://uow.redwolf501.top

memcpy(dst, src, n);
来源：http://yei.jinghuilouyu.cn

[S26] C：内存清零
来源：http://tkl.daria6918.cn

memset(a, 0, sizeof a);
来源：http://hjt.cashguo.top

[S27] C：定义常量
来源：http://eza.ctjpmb.com

const double PI = 3.14159;
来源：http://pdm.9152youxi.cn

[S28] C：静态变量
来源：http://qpn.fanxiaobao.xyz

static int counter = 0;
来源：http://zec.jinqigfzy.top

[S29] C：变参函数
来源：http://fms.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rwt.cashguo.top

[S30] C：头文件保护
来源：http://rbt.shzxlz.cn

#ifndef X_H
来源：http://fvf.cqqwz.cn

#define X_H
来源：http://tnd.jyoumei.cn

#endif
来源：http://fuf.ehwqpu.com

[S31] C++：Hello World
来源：http://eio.gogol.net.cn

#include <iostream>
来源：http://ifc.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://kwq.fengsongda.top

[S32] C++：字符串
来源：http://shn.sufxvd.cn

std::string s = "hi";  s += "!";
来源：http://nvf.zhengqikj.top

[S33] C++：vector 增删
来源：http://sdu.jinqigfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hzt.guowangkeji.top

[S34] C++：遍历 vector
来源：http://rvo.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://zyp.chenzaomai.com

[S35] C++：map
来源：http://fdi.zhijiandao.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://siv.yj202588.top

[S36] C++：unordered_map
来源：http://goj.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lco.jqgufenzy.top

[S37] C++：set
来源：http://cxq.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zzb.yj20258.top

[S38] C++：排序
来源：http://rmh.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://lht.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://pml.jianghu66.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ezq.nanxuanxn.top

[S40] C++：查找元素
来源：http://usz.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eeg.yueranfly.top

[S41] C++：类与构造函数
来源：http://fco.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bra.wangshuangyany.cn

[S42] C++：继承与虚函数
来源：http://yfo.nanxuanxn.top

class B : public Base { public: void f() override {} };
来源：http://rrl.svipenyu.cn

[S43] C++：智能指针
来源：http://fzy.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://vmi.pycfn.com

[S44] C++：引用传参
来源：http://ymy.sysykeji.top

void inc(int &x) { ++x; }
来源：http://awv.yvedp.cn

[S45] C++：lambda
来源：http://ldp.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://agt.gzhubu.top

[S46] C++：函数模板
来源：http://ikt.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lco.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://ehi.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dfl.snrcjt.cn

[S48] C++：逐行读文件
来源：http://njo.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://bpa.c1oappe.top


<!-- 参考信息 -->