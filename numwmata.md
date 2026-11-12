代发 wailian999

[Q61] 移动平均
来源：http://sor.zhoulong.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://biy.feifeiyinyue.top

[Q62] 分组占比
来源：http://kmm.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ocd.tian-w.cn

[Q63] 开启事务
来源：http://hhr.tanke756.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mng.jqgfzy.top

[Q64] 提交事务
来源：http://jjh.yvedp.cn

COMMIT;
来源：http://qeg.zhixingplan.top

[Q65] 回滚事务
来源：http://jii.feifeiyinyue.top

ROLLBACK;
来源：http://otb.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://kde.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nrz.0kj1m.cn

[Q67] 设置隔离级别
来源：http://ssn.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lpt.xylfe.cn

[Q68] 保存点
来源：http://jyb.chenjidiqi.icu

SAVEPOINT sp1;
来源：http://hbd.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://yvo.vehdjk.com

[Q69] 查看执行计划
来源：http://bed.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yft.c1oappe.top

[Q70] 更新统计信息
来源：http://bzr.sxryk.cn

ANALYZE TABLE users;
来源：http://akr.jianghu66.top

[Q71] 查看建表语句
来源：http://fdf.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xij.sxryk.cn

[Q72] 查看索引
来源：http://yey.bbcook.cn

SHOW INDEX FROM users;
来源：http://xwx.yj202588.top

[Q73] 查看表状态
来源：http://nav.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mcp.meibo888.top

[Q74] 强制使用索引
来源：http://gcb.havefunace.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://duh.gogol.net.cn

[Q75] 日期格式化
来源：http://rxm.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yfu.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cyu.pengpengdd.cyou

[Q76] 按天统计
来源：http://qyv.epnwcf.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bwi.nwbrower.top

[Q77] 时间加减
来源：http://nfp.ehwqpu.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gyx.zhijiandao.cn

[Q78] 当前时间
来源：http://lhs.zdqjudy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dpg.sxryk.cn

[Q79] 字符串拼接
来源：http://npe.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ipp.epnwcf.com

[Q80] 字符串截取
来源：http://tuq.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vtw.yvedp.cn

[Q81] 字符串替换
来源：http://wpi.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tsu.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://tcy.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jxn.chenzaomai.com

[Q83] 大小写转换
来源：http://cvp.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gzk.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://qvx.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://ztb.yangfankeji.com

[Q85] 数值取整
来源：http://fwb.zhengqikj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tzk.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://bul.pycfn.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://djd.ivvv.top

[Q87] JSON 字段做条件
来源：http://bch.zhixingplan.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eso.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://ltb.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://teq.jianghu66.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dey.gogol.net.cn

[Q89] 判断表是否存在
来源：http://tht.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cox.ybcxt.top

[Q90] 生成序号列
来源：http://uzh.fengsongda.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xyx.gzhubu.top

================================================================================
来源：http://ble.yvedp.cn

R. Bash 专题
来源：http://jmu.sufxvd.cn

================================================================================
来源：http://qaj.shanyushiyangtech.top

[R01] shebang 与严格模式
来源：http://dmj.jinghuilouyu.cn

#!/usr/bin/env bash
来源：http://cei.52xcode.cn

set -euo pipefail
来源：http://jnh.sxryk.cn

[R02] 变量赋值与使用
来源：http://bje.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://jey.shangyingyoupin.top

[R03] 只读变量
来源：http://ibx.andypj.xyz

readonly PI=3.14
来源：http://icz.ydzc1.top

[R04] 位置参数
来源：http://tsw.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ubw.haohaochexian.top

[R05] 参数默认值
来源：http://zrh.zhaomingkeji.xyz

name="${1:-default}"
来源：http://snv.xylfe.cn

[R06] 判断命令是否存在
来源：http://eno.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://naa.zdbjq.cn

[R07] if 判断文件
来源：http://nnc.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ojl.dianchejie.cn

[R08] 数值比较
来源：http://vsi.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fzx.epnwcf.com

[R09] 字符串比较
来源：http://nqo.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fds.yuanzhike.top

[R10] 正则匹配
来源：http://jio.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qif.jqgfzy.top

[R11] case 多分支
来源：http://ryr.jlsjyb.cn

case "$1" in
来源：http://bez.sysykeji.top

start) echo "启动" ;;
来源：http://szu.guowangkeji.top

stop)  echo "停止" ;;
来源：http://xre.hcnkem.com

*)     echo "未知命令" ;;
来源：http://kie.yueranfly.top

esac
来源：http://yoz.vehdjk.com

[R12] for 遍历文件
来源：http://otq.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://jwa.guannengcc.top

[R13] for 计数循环
来源：http://inl.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://dzw.c1oappe.top

[R14] C 风格 for
来源：http://xhl.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nip.zhengqikj.top

[R15] while 逐行读文件
来源：http://qqb.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qxb.nanxuanxn.top

[R16] until 等待条件
来源：http://zce.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xuj.snrcjt.cn

[R17] 数组定义与取值
来源：http://xde.vqdsnc.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hej.tarul.cn

[R18] 遍历数组
来源：http://win.feifeiyinyue.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://clg.yanxiufei.cn

[R19] 数组长度
来源：http://men.xinyue.icu

echo "${#arr[@]}"
来源：http://zae.vehdjk.com

[R20] 关联数组（字典）
来源：http://ijh.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jlr.smart0.xyz

[R21] 字符串长度
来源：http://tlk.xziqi.cn

echo "${#s}"
来源：http://hgc.shuidangran.top

[R22] 截取子串
来源：http://pld.guannengcc.top

echo "${s:0:5}"
来源：http://yye.ppjwa.cn

[R23] 字符串替换
来源：http://lzf.xingfuxueyuan.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xag.sweek.top

[R24] 大小写转换
来源：http://zpq.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jrx.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://uhu.ppjwa.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jnz.shuidangran.top

[R26] 命令替换
来源：http://hra.bjfxy.top

now=$(date +%F); echo "$now"
来源：http://rod.zhengqikj.top

[R27] 算术展开
来源：http://deo.jinqigfzy.top

echo $((1 + 2 * 3))
来源：http://aju.0kj1m.cn

[R28] 浮点运算
来源：http://egb.zhengqikj.top

echo "scale=2; 10/3" | bc
来源：http://akz.nwbrower.top

[R29] 定义函数
来源：http://vsb.yueranfly.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rrn.bbcook.cn

[R30] 函数返回状态码
来源：http://sya.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://qke.hywenlv.cn

[R31] 局部变量
来源：http://uws.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://una.meibo888.top

[R32] 参数个数校验
来源：http://khw.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wfe.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://iaz.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hqf.xuetiantiany.cn

[R34] 退出时清理
来源：http://kzv.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://ysw.hnqzz.top

[R35] 后台执行并等待
来源：http://chl.hfpthk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kjt.dashuyun.cn

[R36] 并发执行多个任务
来源：http://xpu.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hzh.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://uwr.gotoacloud.top

files=$(ls -1)
来源：http://atr.cqqwz.cn

[R38] 管道串联
来源：http://lpq.feifeiyinyue.top

cat a.txt | grep -i error | wc -l
来源：http://xxg.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://lfh.ydjk.org.cn

cmd > out.log 2>&1
来源：http://wro.kuanghao11.cn

[R40] 追加写日志
来源：http://yfd.tian-w.cn

echo "log" >> out.log
来源：http://hoq.iojbl.cn

[R41] 丢弃输出
来源：http://qqr.guannengcc.top

cmd >/dev/null 2>&1
来源：http://bcu.yonumen.top

[R42] 输入重定向
来源：http://tau.gaohongyu789.top

wc -l < a.txt
来源：http://yty.cheryme.top

[R43] 按名字查找文件
来源：http://grv.hammf.cn

find . -name "*.log" -type f
来源：http://cff.epnwcf.com

[R44] 按修改时间查找
来源：http://pzk.cdnleiting.top

find . -mtime -7 -type f
来源：http://lfc.zhengqikj.top

[R45] 批量删除
来源：http://wgr.xuanzx.com

find . -name "*.tmp" -delete
来源：http://uam.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://jzd.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gmm.gaohongyu789.top

[R47] sed 单行替换
来源：http://qul.yvedp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vda.fehbvm.com

[R48] awk 取指定列
来源：http://cry.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://gcp.uphjek.com

[R49] awk 带条件
来源：http://jkt.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dxt.yueranfly.top

[R50] awk 求和
来源：http://myy.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://bgx.meibo888.top

[R51] 排序去重取前几
来源：http://phf.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://fyd.chenlongwang.top

[R52] 统计行数
来源：http://ozc.ppjwa.cn

wc -l a.txt
来源：http://ggt.shanyushiyangtech.top

[R53] 查看文件头与实时尾
来源：http://wxq.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kpf.sufxvd.cn

[R54] 比较两个文件
来源：http://obe.xziqi.cn

diff a.txt b.txt
来源：http://pud.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://omp.chenlongwang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://shz.ydjk.org.cn

[R56] 远程拷贝
来源：http://zmh.sxryk.cn

scp file user@host:/path/
来源：http://hua.zhengqikj.top

[R57] 远程执行命令
来源：http://mih.dashuyun.cn

ssh user@host 'uptime'
来源：http://snw.cucudq.cn

[R58] 下载文件
来源：http://xee.xuanzx.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xak.fehbvm.com

[R59] 发 POST JSON
来源：http://qtu.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kdm.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://dgk.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ran.cqqwz.cn

[R61] 磁盘占用
来源：http://pdi.yangfankeji.com

df -h;  du -sh *
来源：http://hid.fengsongda.top

[R62] 找最占空间的文件
来源：http://rpe.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://zyf.zhongyouzk.top

[R63] 内存与进程
来源：http://oto.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://olt.nanxinkj.top

[R64] 结束进程
来源：http://cpk.jianghu66.top

kill -9 $(pgrep -f app.py)
来源：http://xxj.ehwqpu.com

[R65] 查看端口占用
来源：http://xev.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://smz.hnxiangtu.top

[R66] 定时任务
来源：http://pwk.iojbl.cn

crontab -e;  crontab -l
来源：http://zru.yongpay.top

[R67] 生成随机十六进制串
来源：http://yvh.uphjek.com

openssl rand -hex 16
来源：http://wlt.sysykeji.top

[R68] 计算文件校验值
来源：http://vdl.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://gol.jiagoushi.top

[R69] 生成随机密码
来源：http://dnt.hnqzz.top

head -c 16 /dev/urandom | base64
来源：http://ybx.hysaishi.cn

[R70] 时间戳与互转
来源：http://epv.zhongyouzk.top

date +%s;  date -d @1700000000
来源：http://wbx.yfazqb.com

[R71] 日期格式化
来源：http://lmi.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vhl.shanyushiyangkeji.top

[R72] 等待端口就绪
来源：http://yvn.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ulb.sysykeji.top

[R73] 分割大日志
来源：http://gce.haohaochexian.top

split -l 1000 big.log part_
来源：http://onx.jqgfzy.top

[R74] 批量重命名
来源：http://rwa.jinqigufen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hhi.aibaodan.cn

[R75] 导出环境变量
来源：http://avb.xuanzx.com

export PATH="$HOME/bin:$PATH"
来源：http://unq.daria6918.cn

[R76] 使用临时文件
来源：http://mha.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://agc.pengpengdd.cyou

[R77] 读取用户输入
来源：http://rvg.haohaochexian.top

read -rp "请输入: " ans
来源：http://usw.ybcxt.top

[R78] 交互式菜单
来源：http://qie.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zrw.guannengcc.top

[R79] 解析命令行选项
来源：http://zrr.gogol.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kfw.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://agv.jinqigufen.top

time ./run.sh
来源：http://iab.yuxming.cn

================================================================================
来源：http://wla.tanke756.top

S. C / C++ 专题
来源：http://uik.fzhhl.top

================================================================================
来源：http://hyl.dashuyun.cn

[S01] C：Hello World
来源：http://upj.epnwcf.com

#include <stdio.h>
来源：http://ovr.chenzaomai.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://pxi.xuanzx.com

[S02] C：变量与格式化输出
来源：http://kky.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://dnj.yj20258888.top

[S03] C：读入整数
来源：http://irq.sysykeji.top

int x; scanf("%d", &x);
来源：http://ojn.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://nzm.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://fpv.ppjwa.cn

[S05] C：字符串长度
来源：http://gyh.zhaomingkeji.xyz

strlen(s)
来源：http://xrv.zdbjq.cn

[S06] C：字符串比较
来源：http://yuu.yuanzhike.top

strcmp(a, b) == 0
来源：http://awl.yangfankeji.com

[S07] C：数组遍历求和
来源：http://gma.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://frh.epnwcf.com

[S08] C：动态内存分配与释放
来源：http://stj.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jhr.yongpay.top

[S09] C：结构体定义与初始化
来源：http://uix.yanxiufei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lly.aibaodan.cn

[S10] C：指针与解引用
来源：http://htk.sweek.top

int *p = &a;  *p = 5;
来源：http://sqa.shangyingyoupin.top

[S11] C：逐行读文件
来源：http://gan.xziqi.cn

FILE *f = fopen("a.txt", "r");
来源：http://eny.yj20258.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yvc.shzxlz.cn

fclose(f);
来源：http://opz.yuxming.cn

[S12] C：写文件
来源：http://yrl.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vhn.bbcook.cn

[S13] C：宏定义
来源：http://wzr.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rqb.cashguo.top

[S14] C：枚举
来源：http://vae.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://ofu.yj202588.top

[S15] C：类型转换
来源：http://gxb.svipenyu.cn

(double) a / b
来源：http://hyq.wangshuangyany.cn

[S16] C：位操作置位
来源：http://mva.dashuyun.cn

x |= (1 << 3);
来源：http://jjm.fehbvm.com

[S17] C：安全拼接字符串
来源：http://bsy.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hkl.hnqzz.top

[S18] C：命令行参数
来源：http://zwg.xylfe.cn

int main(int argc, char **argv)
来源：http://pxe.xinyue.icu

[S19] C：快速排序
来源：http://vzd.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://peq.andypj.xyz

[S20] C：二分查找
来源：http://enc.gaohongyu789.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ymt.zhixingplan.top

[S21] C：字符类别判断
来源：http://byb.zhixingplan.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hkn.52xcode.cn

[S22] C：字符串转数字
来源：http://crx.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rms.bbcook.cn

[S23] C：随机数
来源：http://sko.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ttq.smart0.xyz

[S24] C：获取本地时间
来源：http://ixo.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bym.gotoacloud.top

[S25] C：内存拷贝
来源：http://tuv.zdbjq.cn

memcpy(dst, src, n);
来源：http://sez.fanxiaobao.xyz

[S26] C：内存清零
来源：http://dtp.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://wkv.gogol.net.cn

[S27] C：定义常量
来源：http://wwu.yanxiufei.cn

const double PI = 3.14159;
来源：http://hlk.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://snw.wangshuangyany.cn

static int counter = 0;
来源：http://cdg.yfazqb.com

[S29] C：变参函数
来源：http://ncd.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sgz.gogol.net.cn

[S30] C：头文件保护
来源：http://lmz.hcnkem.com

#ifndef X_H
来源：http://hea.sufxvd.cn

#define X_H
来源：http://vio.guowangkeji.top

#endif
来源：http://ybi.tarul.cn

[S31] C++：Hello World
来源：http://vod.gotoacloud.top


<!-- 参考信息 -->