代发 wailian999

[Q67] 设置隔离级别
来源：http://cnx.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zwg.haohaochexian.top

[Q68] 保存点
来源：http://exg.316326.xyz

SAVEPOINT sp1;
来源：http://svx.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://nfl.c1oappe.top

[Q69] 查看执行计划
来源：http://zzs.vehdjk.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gqn.yuanzhike.top

[Q70] 更新统计信息
来源：http://zsx.xingfuxueyuan.xyz

ANALYZE TABLE users;
来源：http://ixt.shangyingyoupin.top

[Q71] 查看建表语句
来源：http://pwh.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vzd.fanxiaobao.xyz

[Q72] 查看索引
来源：http://fvj.zhaomingkeji.xyz

SHOW INDEX FROM users;
来源：http://uew.zdbjq.cn

[Q73] 查看表状态
来源：http://rhq.wangdashe.top

SHOW TABLE STATUS LIKE 'users';
来源：http://prt.ydjk.org.cn

[Q74] 强制使用索引
来源：http://tqs.yj202588.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sbh.ppjwa.cn

[Q75] 日期格式化
来源：http://uop.birdmap.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ghj.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qeu.ybcxt.top

[Q76] 按天统计
来源：http://mco.zhijiandao.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nxz.gzhubu.top

[Q77] 时间加减
来源：http://omw.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uzo.hammf.cn

[Q78] 当前时间
来源：http://vnk.sysykeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ylj.yj202588.top

[Q79] 字符串拼接
来源：http://onx.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ojb.nanxinkj.top

[Q80] 字符串截取
来源：http://kkp.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://otv.nanxuanxn.top

[Q81] 字符串替换
来源：http://lru.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ypw.tanke756.top

[Q82] 字符长度与字节长度
来源：http://cyq.zycfv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yoy.chenlongwang.top

[Q83] 大小写转换
来源：http://hdf.hnxiangtu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mpn.fengsongda.top

[Q84] 去除首尾空格
来源：http://wpu.uphjek.com

SELECT TRIM(name) FROM users;
来源：http://cdv.tarul.cn

[Q85] 数值取整
来源：http://wze.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dlq.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://qjz.wangshuangyany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vzd.xuanzx.com

[Q87] JSON 字段做条件
来源：http://qep.yueranfly.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ima.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://qxq.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xnp.jlsjyb.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kfu.feifeiyinyue.top

[Q89] 判断表是否存在
来源：http://ewm.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jji.sufxvd.cn

[Q90] 生成序号列
来源：http://xdx.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mhf.52xcode.cn

================================================================================
来源：http://mbg.jiagoushi.top

R. Bash 专题
来源：http://nku.sufxvd.cn

================================================================================
来源：http://xwo.jinqigufen.top

[R01] shebang 与严格模式
来源：http://fhn.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://tzt.yj202588.top

set -euo pipefail
来源：http://wjc.bbcook.cn

[R02] 变量赋值与使用
来源：http://icq.yuanzhike.top

name="Tom"; echo "$name"
来源：http://flf.shanyushiyangtech.top

[R03] 只读变量
来源：http://rdp.hnxiangtu.top

readonly PI=3.14
来源：http://xzq.hesvh.cn

[R04] 位置参数
来源：http://llk.ydjk.org.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tux.feifeiyinyue.top

[R05] 参数默认值
来源：http://pns.jinyuanbaomall.cn

name="${1:-default}"
来源：http://ipd.hcnkem.com

[R06] 判断命令是否存在
来源：http://hmx.tarul.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hvg.haohaochexian.top

[R07] if 判断文件
来源：http://zhm.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://asp.cheryme.top

[R08] 数值比较
来源：http://fev.yfazqb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://wdg.yuxming.cn

[R09] 字符串比较
来源：http://bxq.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lva.xziqi.cn

[R10] 正则匹配
来源：http://dzz.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xpg.wangdashe.top

[R11] case 多分支
来源：http://sto.zhaomingkeji.xyz

case "$1" in
来源：http://vmz.uphjek.com

start) echo "启动" ;;
来源：http://tun.chenlongwang.top

stop)  echo "停止" ;;
来源：http://mgk.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://tll.zhongyouzk.top

esac
来源：http://slz.yuxming.cn

[R12] for 遍历文件
来源：http://cac.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://fsp.sufxvd.cn

[R13] for 计数循环
来源：http://vcn.hywenlv.cn

for i in {1..10}; do echo "$i"; done
来源：http://apx.dianchejie.cn

[R14] C 风格 for
来源：http://mbf.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nue.c1oappe.top

[R15] while 逐行读文件
来源：http://dvw.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ajc.dashuyun.cn

[R16] until 等待条件
来源：http://mko.meibo888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zpv.jiagoushi.top

[R17] 数组定义与取值
来源：http://gxh.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ksv.shuidangran.top

[R18] 遍历数组
来源：http://bay.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mof.jyoumei.cn

[R19] 数组长度
来源：http://tme.hammf.cn

echo "${#arr[@]}"
来源：http://yni.zdbjq.cn

[R20] 关联数组（字典）
来源：http://mto.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cws.ehwqpu.com

[R21] 字符串长度
来源：http://orh.316326.xyz

echo "${#s}"
来源：http://rtd.svipenyu.cn

[R22] 截取子串
来源：http://vub.jiagoushi.top

echo "${s:0:5}"
来源：http://eck.yj202588.top

[R23] 字符串替换
来源：http://xce.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lds.jqgfzy.top

[R24] 大小写转换
来源：http://cxk.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://zsv.hnxiangtu.top

[R25] 去后缀 / 去前缀
来源：http://oeb.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tby.shuidangran.top

[R26] 命令替换
来源：http://zlo.uphjek.com

now=$(date +%F); echo "$now"
来源：http://dsa.yongpay.top

[R27] 算术展开
来源：http://zsx.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://olx.dashuyun.cn

[R28] 浮点运算
来源：http://quw.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://oli.vqdsnc.cn

[R29] 定义函数
来源：http://for.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://amx.meibo888.top

[R30] 函数返回状态码
来源：http://mpi.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://xix.nanxinkj.top

[R31] 局部变量
来源：http://vly.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://skg.ydjk.org.cn

[R32] 参数个数校验
来源：http://dgx.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lor.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://wtg.fktsv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eru.yj20258.top

[R34] 退出时清理
来源：http://hpq.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://hci.aibaodan.cn

[R35] 后台执行并等待
来源：http://qnv.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rbn.9152youxi.cn

[R36] 并发执行多个任务
来源：http://fiu.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ims.jinqigufen.top

[R37] 把输出赋给变量
来源：http://zgt.yvedp.cn

files=$(ls -1)
来源：http://uzx.kuanghao11.cn

[R38] 管道串联
来源：http://xfx.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://bdg.zhixingplan.top

[R39] 重定向标准输出与错误
来源：http://miu.epnwcf.com

cmd > out.log 2>&1
来源：http://off.daria6918.cn

[R40] 追加写日志
来源：http://kqy.shuidangran.top

echo "log" >> out.log
来源：http://wcw.shangyingyoupin.top

[R41] 丢弃输出
来源：http://hxo.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://yqu.sufxvd.cn

[R42] 输入重定向
来源：http://vlb.gogol.net.cn

wc -l < a.txt
来源：http://sog.wangdashe.top

[R43] 按名字查找文件
来源：http://jum.jiagoushi.top

find . -name "*.log" -type f
来源：http://hib.ydjk.org.cn

[R44] 按修改时间查找
来源：http://jdw.xuanzx.com

find . -mtime -7 -type f
来源：http://djf.shuidangran.top

[R45] 批量删除
来源：http://qfj.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://uvs.hesvh.cn

[R46] 递归替换文件内容
来源：http://pyd.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yhh.epnwcf.com

[R47] sed 单行替换
来源：http://pey.xziqi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qvp.yvedp.cn

[R48] awk 取指定列
来源：http://ype.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://bac.svipenyu.cn

[R49] awk 带条件
来源：http://wyh.uphjek.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aet.aizwys.cn

[R50] awk 求和
来源：http://tvb.52xcode.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rjo.xuanzx.com

[R51] 排序去重取前几
来源：http://ayp.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jkw.sysykeji.top

[R52] 统计行数
来源：http://ick.ppjwa.cn

wc -l a.txt
来源：http://rtk.shanyushiyangtech.top

[R53] 查看文件头与实时尾
来源：http://fuk.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://szr.hnxiangtu.top

[R54] 比较两个文件
来源：http://twg.yj20258888.top

diff a.txt b.txt
来源：http://uzj.cashguo.top

[R55] 压缩与解压
来源：http://hhz.chenlongwang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wxl.tianlin.xyz

[R56] 远程拷贝
来源：http://jvy.smart0.xyz

scp file user@host:/path/
来源：http://gye.zhongyouzk.top

[R57] 远程执行命令
来源：http://gvb.yj202588.top

ssh user@host 'uptime'
来源：http://qvh.hesvh.cn

[R58] 下载文件
来源：http://oum.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hfh.nanxinkj.top

[R59] 发 POST JSON
来源：http://mtt.xziqi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zoc.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://uga.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iuo.feifeiyinyue.top

[R61] 磁盘占用
来源：http://aem.daria6918.cn

df -h;  du -sh *
来源：http://uwk.andypj.xyz

[R62] 找最占空间的文件
来源：http://kjw.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://vee.shangyingyoupin.top

[R63] 内存与进程
来源：http://byz.dashuyun.cn

free -h;  ps aux | grep nginx
来源：http://wys.yuxming.cn

[R64] 结束进程
来源：http://lup.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://wyf.aibaodan.cn

[R65] 查看端口占用
来源：http://kfx.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sfl.meibo888.top

[R66] 定时任务
来源：http://vog.sjlbkw.cn

crontab -e;  crontab -l
来源：http://xel.vqdsnc.cn

[R67] 生成随机十六进制串
来源：http://mfh.zdbjq.cn

openssl rand -hex 16
来源：http://qxi.quarkkingdee.top

[R68] 计算文件校验值
来源：http://mfb.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://gol.zycfv.cn

[R69] 生成随机密码
来源：http://hue.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://odn.pycfn.com

[R70] 时间戳与互转
来源：http://ktf.sjlbkw.cn

date +%s;  date -d @1700000000
来源：http://njt.hnqzz.top

[R71] 日期格式化
来源：http://hta.yueranfly.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nbv.guannengcc.top

[R72] 等待端口就绪
来源：http://gsz.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hfj.uphjek.com

[R73] 分割大日志
来源：http://ubv.havefunace.top

split -l 1000 big.log part_
来源：http://xge.feifeiyinyue.top

[R74] 批量重命名
来源：http://mds.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gqk.smart0.xyz

[R75] 导出环境变量
来源：http://kzx.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://eyo.zhoulong.xyz

[R76] 使用临时文件
来源：http://eux.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qxy.yfazqb.com

[R77] 读取用户输入
来源：http://hgx.ivvv.top

read -rp "请输入: " ans
来源：http://hhi.jqgufenzy.top

[R78] 交互式菜单
来源：http://plz.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://ytu.yangfankeji.com

[R79] 解析命令行选项
来源：http://dny.yueranfly.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://afd.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://szm.pycfn.com

time ./run.sh
来源：http://hwt.cashguo.top

================================================================================
来源：http://ljl.hammf.cn

S. C / C++ 专题
来源：http://frc.fanxiaobao.xyz

================================================================================
来源：http://ghy.dashuyun.cn

[S01] C：Hello World
来源：http://rpc.andypj.xyz

#include <stdio.h>
来源：http://ztc.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ffw.cashguo.top

[S02] C：变量与格式化输出
来源：http://diy.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://mvo.zhoulong.xyz

[S03] C：读入整数
来源：http://fuf.yfazqb.com

int x; scanf("%d", &x);
来源：http://izh.mhx1999.top

[S04] C：字符串复制
来源：http://cdl.feifeiyinyue.top

char dst[32]; strcpy(dst, "hi");
来源：http://pjw.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://tca.feifeiyinyue.top

strlen(s)
来源：http://dxo.yuanzhike.top

[S06] C：字符串比较
来源：http://iul.yangfankeji.com

strcmp(a, b) == 0
来源：http://ebo.nwbrower.top

[S07] C：数组遍历求和
来源：http://svp.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://soe.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://xka.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rce.yj20258888.top

[S09] C：结构体定义与初始化
来源：http://qhf.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://akf.epnwcf.com

[S10] C：指针与解引用
来源：http://lua.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://viw.jiagoushi.top

[S11] C：逐行读文件
来源：http://pjg.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://suq.ctjpmb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ngj.52xcode.cn

fclose(f);
来源：http://xex.cucudq.cn

[S12] C：写文件
来源：http://ahf.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yum.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://fmc.aibaodan.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sqe.svipenyu.cn

[S14] C：枚举
来源：http://jhy.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://msw.fktsv.cn

[S15] C：类型转换
来源：http://sar.aizwys.cn

(double) a / b
来源：http://zgi.fanxiaobao.xyz

[S16] C：位操作置位
来源：http://yoi.ppjwa.cn

x |= (1 << 3);
来源：http://ewc.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://cef.sysykeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vms.fehbvm.com

[S18] C：命令行参数
来源：http://ely.nwbrower.top

int main(int argc, char **argv)
来源：http://uib.gaohongyu789.top

[S19] C：快速排序
来源：http://jqp.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uje.havefunace.top

[S20] C：二分查找
来源：http://ghi.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hvf.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://lsy.sweek.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dfj.dianchejie.cn

[S22] C：字符串转数字
来源：http://gmf.zhaomingkeji.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://opo.fktsv.cn

[S23] C：随机数
来源：http://iki.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://vog.xuanzx.com

[S24] C：获取本地时间
来源：http://yyz.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mxz.316326.xyz

[S25] C：内存拷贝
来源：http://xsd.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://vvv.gzhubu.top

[S26] C：内存清零
来源：http://qmf.fktsv.cn

memset(a, 0, sizeof a);
来源：http://cfo.chenjidiqi.icu

[S27] C：定义常量
来源：http://vyz.zdbjq.cn

const double PI = 3.14159;
来源：http://qsb.feifeiyinyue.top

[S28] C：静态变量
来源：http://den.bjfxy.top

static int counter = 0;
来源：http://swa.316326.xyz

[S29] C：变参函数
来源：http://gyo.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pdj.hysaishi.cn

[S30] C：头文件保护
来源：http://hdk.zdqjudy.top

#ifndef X_H
来源：http://lvt.cashguo.top

#define X_H
来源：http://hhu.uphjek.com

#endif
来源：http://ict.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://vcf.yj20258.top

#include <iostream>
来源：http://ppn.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://xco.wangdashe.top

[S32] C++：字符串
来源：http://wzq.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://hiv.meibo888.top

[S33] C++：vector 增删
来源：http://her.yvedp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://djy.cheryme.top

[S34] C++：遍历 vector
来源：http://kyj.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://btz.havefunace.top

[S35] C++：map
来源：http://irr.tanke756.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wdb.jinqigfzy.top

[S36] C++：unordered_map
来源：http://fuy.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uaw.zdbjq.cn


<!-- 参考信息 -->