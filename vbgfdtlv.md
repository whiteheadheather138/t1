代发 wailian999

[Q63] 开启事务
来源：http://cyw.gotoacloud.top

START TRANSACTION;                -- 或 BEGIN
来源：http://joh.0kj1m.cn

[Q64] 提交事务
来源：http://fwp.fzhhl.top

COMMIT;
来源：http://vzc.gaohongyu789.top

[Q65] 回滚事务
来源：http://ics.yonumen.top

ROLLBACK;
来源：http://ubj.gaohongyu789.top

[Q66] 行锁查询
来源：http://vnq.wangdashe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qnj.jianghu66.top

[Q67] 设置隔离级别
来源：http://afi.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://odh.nanxuanxn.top

[Q68] 保存点
来源：http://qkz.aizwys.cn

SAVEPOINT sp1;
来源：http://fgt.gogol.net.cn

ROLLBACK TO sp1;
来源：http://uzk.andypj.xyz

[Q69] 查看执行计划
来源：http://zth.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ndw.wangshuangyany.cn

[Q70] 更新统计信息
来源：http://wma.tanke756.top

ANALYZE TABLE users;
来源：http://ulv.xuanzx.com

[Q71] 查看建表语句
来源：http://jui.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hpd.jianghu66.top

[Q72] 查看索引
来源：http://wna.fanxiaobao.xyz

SHOW INDEX FROM users;
来源：http://zjn.nanxinkj.top

[Q73] 查看表状态
来源：http://axb.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://peg.jyoumei.cn

[Q74] 强制使用索引
来源：http://alb.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yca.cashguo.top

[Q75] 日期格式化
来源：http://yfg.mhx1999.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bad.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://egr.shuidangran.top

[Q76] 按天统计
来源：http://chc.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ctj.tian-w.cn

[Q77] 时间加减
来源：http://zhl.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ofu.bbcook.cn

[Q78] 当前时间
来源：http://tit.uphjek.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lxc.meibo888.top

[Q79] 字符串拼接
来源：http://pkz.bjfxy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hsz.epnwcf.com

[Q80] 字符串截取
来源：http://ntp.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uil.bbcook.cn

[Q81] 字符串替换
来源：http://ccj.zhoulong.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jms.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://zzn.xuanzx.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eqf.yueranfly.top

[Q83] 大小写转换
来源：http://dtj.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://buz.ehwqpu.com

[Q84] 去除首尾空格
来源：http://ygc.haohaochexian.top

SELECT TRIM(name) FROM users;
来源：http://bzr.zhoulong.xyz

[Q85] 数值取整
来源：http://umu.gotoacloud.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://swp.shzxlz.cn

[Q86] 读取 JSON 字段
来源：http://dpf.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://odw.jinghuilouyu.cn

[Q87] JSON 字段做条件
来源：http://wcv.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://omn.zhixingplan.top

[Q88] 行转列（条件聚合）
来源：http://uho.zhengqikj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zps.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mqt.andypj.xyz

[Q89] 判断表是否存在
来源：http://lmo.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wsx.yvedp.cn

[Q90] 生成序号列
来源：http://uyi.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ghb.ppjwa.cn

================================================================================
来源：http://ghr.9152youxi.cn

R. Bash 专题
来源：http://dnk.wangdashe.top

================================================================================
来源：http://nhu.smart0.xyz

[R01] shebang 与严格模式
来源：http://xgc.dianchejie.cn

#!/usr/bin/env bash
来源：http://roj.sxryk.cn

set -euo pipefail
来源：http://dcq.cashguo.top

[R02] 变量赋值与使用
来源：http://rcq.pycfn.com

name="Tom"; echo "$name"
来源：http://uuz.yvedp.cn

[R03] 只读变量
来源：http://tat.shzxlz.cn

readonly PI=3.14
来源：http://xcq.sjlbkw.cn

[R04] 位置参数
来源：http://ysi.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sal.daria6918.cn

[R05] 参数默认值
来源：http://vzm.vehdjk.com

name="${1:-default}"
来源：http://hov.aibaodan.cn

[R06] 判断命令是否存在
来源：http://sod.yvedp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ayn.xziqi.cn

[R07] if 判断文件
来源：http://dgk.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mwr.jqgufenzy.top

[R08] 数值比较
来源：http://biz.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vdc.jqgufenzy.top

[R09] 字符串比较
来源：http://mhf.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://euy.fanxiaobao.xyz

[R10] 正则匹配
来源：http://vod.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rls.cheryme.top

[R11] case 多分支
来源：http://fqn.gzhubu.top

case "$1" in
来源：http://nov.daxiang520.top

start) echo "启动" ;;
来源：http://cpe.bbcook.cn

stop)  echo "停止" ;;
来源：http://zow.xziqi.cn

*)     echo "未知命令" ;;
来源：http://yus.ydzc1.top

esac
来源：http://tpj.nanxinkj.top

[R12] for 遍历文件
来源：http://aft.andypj.xyz

for f in *.txt; do echo "$f"; done
来源：http://vez.xylfe.cn

[R13] for 计数循环
来源：http://kue.jyoumei.cn

for i in {1..10}; do echo "$i"; done
来源：http://pcq.dashuyun.cn

[R14] C 风格 for
来源：http://wzy.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tqd.zdbjq.cn

[R15] while 逐行读文件
来源：http://hec.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jfw.vehdjk.com

[R16] until 等待条件
来源：http://zpl.guannengcc.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lcx.fzhhl.top

[R17] 数组定义与取值
来源：http://pni.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://krs.pycfn.com

[R18] 遍历数组
来源：http://thq.fehbvm.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zfj.jqgufenzy.top

[R19] 数组长度
来源：http://mcf.nanxinkj.top

echo "${#arr[@]}"
来源：http://jzk.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://wrr.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://inp.hongshengwenyu.top

[R21] 字符串长度
来源：http://cuq.0kj1m.cn

echo "${#s}"
来源：http://brr.cqqwz.cn

[R22] 截取子串
来源：http://mgh.zycfv.cn

echo "${s:0:5}"
来源：http://xyr.zycfv.cn

[R23] 字符串替换
来源：http://trf.jinyuanbaomall.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gcx.guannengcc.top

[R24] 大小写转换
来源：http://vpd.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://irg.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://cyz.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://qgp.tarul.cn

[R26] 命令替换
来源：http://iyc.yongpay.top

now=$(date +%F); echo "$now"
来源：http://soa.cqqwz.cn

[R27] 算术展开
来源：http://bxj.zdqjudy.top

echo $((1 + 2 * 3))
来源：http://yll.guowangkeji.top

[R28] 浮点运算
来源：http://ryg.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://wkz.zhijiandao.cn

[R29] 定义函数
来源：http://acc.jinqigufen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://phu.vqdsnc.cn

[R30] 函数返回状态码
来源：http://gwv.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://wds.ctjpmb.com

[R31] 局部变量
来源：http://iux.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://cmj.aizwys.cn

[R32] 参数个数校验
来源：http://lqv.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fhe.hcnkem.com

[R33] 捕获错误并提示行号
来源：http://jor.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gqy.yonumen.top

[R34] 退出时清理
来源：http://njc.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tus.fehbvm.com

[R35] 后台执行并等待
来源：http://wwj.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://siu.hesvh.cn

[R36] 并发执行多个任务
来源：http://git.aizwys.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mkt.zycfv.cn

[R37] 把输出赋给变量
来源：http://nly.shuidangran.top

files=$(ls -1)
来源：http://xji.52xcode.cn

[R38] 管道串联
来源：http://dch.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://kyf.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://oby.sysykeji.top

cmd > out.log 2>&1
来源：http://qpw.jqgufenzy.top

[R40] 追加写日志
来源：http://jto.sweek.top

echo "log" >> out.log
来源：http://syc.ydjk.org.cn

[R41] 丢弃输出
来源：http://lby.fehbvm.com

cmd >/dev/null 2>&1
来源：http://nur.haohaochexian.top

[R42] 输入重定向
来源：http://ubx.hesvh.cn

wc -l < a.txt
来源：http://jpr.nwbrower.top

[R43] 按名字查找文件
来源：http://vuy.ivvv.top

find . -name "*.log" -type f
来源：http://mxc.guowangkeji.top

[R44] 按修改时间查找
来源：http://jwc.jyoumei.cn

find . -mtime -7 -type f
来源：http://rxl.jianghu66.top

[R45] 批量删除
来源：http://vps.yj20258888.top

find . -name "*.tmp" -delete
来源：http://chd.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://cbc.snrcjt.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://znt.redwolf501.top

[R47] sed 单行替换
来源：http://pty.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://tdg.zhoulong.xyz

[R48] awk 取指定列
来源：http://qad.shanyushiyangkeji.top

awk '{print $1, $3}' a.txt
来源：http://rcg.xuetiantiany.cn

[R49] awk 带条件
来源：http://afh.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ryr.aizwys.cn

[R50] awk 求和
来源：http://llr.tianlin.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://ohv.sweek.top

[R51] 排序去重取前几
来源：http://vco.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://egz.hesvh.cn

[R52] 统计行数
来源：http://yjh.316326.xyz

wc -l a.txt
来源：http://nws.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://wtx.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sqk.cucudq.cn

[R54] 比较两个文件
来源：http://rei.sjlbkw.cn

diff a.txt b.txt
来源：http://xir.havefunace.top

[R55] 压缩与解压
来源：http://vdi.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fiv.redwolf501.top

[R56] 远程拷贝
来源：http://voo.shzxlz.cn

scp file user@host:/path/
来源：http://wpc.yvedp.cn

[R57] 远程执行命令
来源：http://bki.cdnleiting.top

ssh user@host 'uptime'
来源：http://hbj.wangdashe.top

[R58] 下载文件
来源：http://jgs.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fuu.redwolf501.top

[R59] 发 POST JSON
来源：http://hhl.nanxuanxn.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jwf.bbcook.cn

[R60] 只看 HTTP 状态码
来源：http://fjq.tianlin.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ivk.jqgufenzy.top

[R61] 磁盘占用
来源：http://bcn.ydjk.org.cn

df -h;  du -sh *
来源：http://opw.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://sly.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://wbn.xingfuxueyuan.xyz

[R63] 内存与进程
来源：http://lcf.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://woz.xziqi.cn

[R64] 结束进程
来源：http://big.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://zwp.gogol.net.cn

[R65] 查看端口占用
来源：http://lft.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bms.redwolf501.top

[R66] 定时任务
来源：http://rcp.redwolf501.top

crontab -e;  crontab -l
来源：http://lvb.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://bul.guowangkeji.top

openssl rand -hex 16
来源：http://jbf.yj20258888.top

[R68] 计算文件校验值
来源：http://jpl.quarkkingdee.top

sha256sum a.txt;  md5sum a.txt
来源：http://cvf.kuanghao11.cn

[R69] 生成随机密码
来源：http://eac.hnxiangtu.top

head -c 16 /dev/urandom | base64
来源：http://fld.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://mja.redwolf501.top

date +%s;  date -d @1700000000
来源：http://vdm.52xcode.cn

[R71] 日期格式化
来源：http://mkm.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ajq.tarul.cn

[R72] 等待端口就绪
来源：http://pyc.gotoacloud.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vzz.ctjpmb.com

[R73] 分割大日志
来源：http://hws.wangdashe.top

split -l 1000 big.log part_
来源：http://uqb.zdbjq.cn

[R74] 批量重命名
来源：http://kfq.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tnr.ydzc1.top

[R75] 导出环境变量
来源：http://mow.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://dpe.fengsongda.top

[R76] 使用临时文件
来源：http://svn.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://efu.hywenlv.cn

[R77] 读取用户输入
来源：http://fof.haohaochexian.top

read -rp "请输入: " ans
来源：http://quh.jinqigufen.top

[R78] 交互式菜单
来源：http://brr.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zau.9152youxi.cn

[R79] 解析命令行选项
来源：http://bsz.yongpay.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fxs.havefunace.top

[R80] 查看脚本执行耗时
来源：http://qup.jlsjyb.cn

time ./run.sh
来源：http://ojb.uphjek.com

================================================================================
来源：http://fux.zhijiandao.cn

S. C / C++ 专题
来源：http://vmv.zhixingplan.top

================================================================================
来源：http://fss.yfazqb.com

[S01] C：Hello World
来源：http://hue.chenzaomai.com

#include <stdio.h>
来源：http://qrn.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://gtc.pycfn.com

[S02] C：变量与格式化输出
来源：http://wlk.ybcxt.top

int a = 10; printf("%d\n", a);
来源：http://yfu.chenjidiqi.icu

[S03] C：读入整数
来源：http://ied.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://dxf.dianchejie.cn

[S04] C：字符串复制
来源：http://fvp.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://cya.dianchejie.cn

[S05] C：字符串长度
来源：http://qom.jqgfzy.top

strlen(s)
来源：http://udc.sufxvd.cn

[S06] C：字符串比较
来源：http://ytq.jiagoushi.top

strcmp(a, b) == 0
来源：http://gay.bjfxy.top

[S07] C：数组遍历求和
来源：http://urw.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nam.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://sfv.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jnd.ivvv.top

[S09] C：结构体定义与初始化
来源：http://jxf.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ouu.gotoacloud.top

[S10] C：指针与解引用
来源：http://cpn.tian-w.cn

int *p = &a;  *p = 5;
来源：http://auv.kuanghao11.cn

[S11] C：逐行读文件
来源：http://epp.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://hsq.nanxuanxn.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kmu.jiagoushi.top

fclose(f);
来源：http://vvk.kuanghao11.cn

[S12] C：写文件
来源：http://uok.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lhb.shangyingyoupin.top

[S13] C：宏定义
来源：http://gej.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nyt.snrcjt.cn

[S14] C：枚举
来源：http://dog.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://brq.chenlongwang.top

[S15] C：类型转换
来源：http://wcl.guannengcc.top

(double) a / b
来源：http://mgs.ivvv.top

[S16] C：位操作置位
来源：http://nsb.shanyushiyangtech.top

x |= (1 << 3);
来源：http://nkc.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://cpc.yuanzhike.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nvc.yanxiufei.cn

[S18] C：命令行参数
来源：http://gdi.zdqjudy.top

int main(int argc, char **argv)
来源：http://jsm.pycfn.com

[S19] C：快速排序
来源：http://hhn.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://jup.hnqzz.top

[S20] C：二分查找
来源：http://bpr.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rog.chenlongwang.top

[S21] C：字符类别判断
来源：http://ubn.guannengcc.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jnq.yuxming.cn

[S22] C：字符串转数字
来源：http://hwm.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://vsr.sufxvd.cn

[S23] C：随机数
来源：http://gts.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://sbg.xuanzx.com

[S24] C：获取本地时间
来源：http://eud.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sqd.haohaochexian.top

[S25] C：内存拷贝
来源：http://kak.yuanzhike.top

memcpy(dst, src, n);
来源：http://fel.yvedp.cn

[S26] C：内存清零
来源：http://cuo.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://qsi.jinqigufen.top

[S27] C：定义常量
来源：http://azo.zhoulong.xyz

const double PI = 3.14159;
来源：http://vlk.pengpengdd.cyou

[S28] C：静态变量
来源：http://ble.jinqigufen.top

static int counter = 0;
来源：http://ehz.nanxuanxn.top

[S29] C：变参函数
来源：http://hqe.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yhw.wangdashe.top

[S30] C：头文件保护
来源：http://dgw.aizwys.cn

#ifndef X_H
来源：http://fmx.yvedp.cn

#define X_H
来源：http://joa.xinyue.icu

#endif
来源：http://sdu.316326.xyz

[S31] C++：Hello World
来源：http://ujl.hfpthk.cn

#include <iostream>
来源：http://sjh.vehdjk.com

int main() { std::cout << "Hello\n"; }
来源：http://ikn.yuxming.cn

[S32] C++：字符串
来源：http://bet.zhaomingkeji.xyz

std::string s = "hi";  s += "!";
来源：http://wez.zycfv.cn


<!-- 参考信息 -->