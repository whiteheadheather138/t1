代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://igw.yueranfly.top

[Q54] 清空表
来源：http://yfr.bbcook.cn

TRUNCATE TABLE logs;
来源：http://mzg.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://ttm.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://edg.yangfankeji.com

[Q56] 密集排名（并列不占位）
来源：http://cxf.zdqjudy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iit.zdbjq.cn

[Q57] 行号
来源：http://bal.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tgu.jlsjyb.cn

[Q58] 累计求和
来源：http://rqx.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gor.zycfv.cn

[Q59] 分组内累计
来源：http://xdi.fehbvm.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vvo.xziqi.cn

[Q60] 取上一行 / 下一行
来源：http://fln.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tnt.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tah.zycfv.cn

[Q61] 移动平均
来源：http://ivf.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ocy.xinyue.icu

[Q62] 分组占比
来源：http://ore.wangshuangyany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tes.zycfv.cn

[Q63] 开启事务
来源：http://ddj.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dhu.feifeiyinyue.top

[Q64] 提交事务
来源：http://fav.yj20258.top

COMMIT;
来源：http://gga.epnwcf.com

[Q65] 回滚事务
来源：http://hcs.xuetiantiany.cn

ROLLBACK;
来源：http://jwi.yuanzhike.top

[Q66] 行锁查询
来源：http://pxd.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mjo.cdnleiting.top

[Q67] 设置隔离级别
来源：http://nqr.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fgz.jianghu66.top

[Q68] 保存点
来源：http://iom.hywenlv.cn

SAVEPOINT sp1;
来源：http://rzn.andypj.xyz

ROLLBACK TO sp1;
来源：http://ree.jiagoushi.top

[Q69] 查看执行计划
来源：http://uxi.hcnkem.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mkg.zhijiandao.cn

[Q70] 更新统计信息
来源：http://bwn.yj202588.top

ANALYZE TABLE users;
来源：http://yoy.c1oappe.top

[Q71] 查看建表语句
来源：http://rpd.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uia.xylfe.cn

[Q72] 查看索引
来源：http://dpg.zhixingplan.top

SHOW INDEX FROM users;
来源：http://aiq.birdmap.top

[Q73] 查看表状态
来源：http://qkg.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wja.ivvv.top

[Q74] 强制使用索引
来源：http://qkc.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aoz.chenlongwang.top

[Q75] 日期格式化
来源：http://fjh.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zxl.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oce.xziqi.cn

[Q76] 按天统计
来源：http://jfa.sweek.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dxy.xingfuxueyuan.xyz

[Q77] 时间加减
来源：http://nyo.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uel.bjfxy.top

[Q78] 当前时间
来源：http://wtl.pycfn.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nwh.cheryme.top

[Q79] 字符串拼接
来源：http://hjk.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vvv.cucudq.cn

[Q80] 字符串截取
来源：http://zoe.zhoulong.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rnx.jyoumei.cn

[Q81] 字符串替换
来源：http://ehg.zhijiandao.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dci.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://uvq.zdbjq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://urh.zdbjq.cn

[Q83] 大小写转换
来源：http://flx.uphjek.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ysu.fehbvm.com

[Q84] 去除首尾空格
来源：http://wxj.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://fum.feifeiyinyue.top

[Q85] 数值取整
来源：http://xcu.aizwys.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tix.jianghu66.top

[Q86] 读取 JSON 字段
来源：http://cun.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eqw.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://ern.ehwqpu.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nsf.gzhubu.top

[Q88] 行转列（条件聚合）
来源：http://niy.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nhx.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cdf.epnwcf.com

[Q89] 判断表是否存在
来源：http://jib.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nsk.9152youxi.cn

[Q90] 生成序号列
来源：http://ptr.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ier.nanxinkj.top

================================================================================
来源：http://ynz.ivvv.top

R. Bash 专题
来源：http://nmm.jiagoushi.top

================================================================================
来源：http://iqs.shzxlz.cn

[R01] shebang 与严格模式
来源：http://bam.xziqi.cn

#!/usr/bin/env bash
来源：http://lez.9152youxi.cn

set -euo pipefail
来源：http://kvx.ppjwa.cn

[R02] 变量赋值与使用
来源：http://gty.havefunace.top

name="Tom"; echo "$name"
来源：http://soi.jqgfzy.top

[R03] 只读变量
来源：http://ibg.ivvv.top

readonly PI=3.14
来源：http://zfq.ivvv.top

[R04] 位置参数
来源：http://pxe.chenjidiqi.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fvz.wangshuangyany.cn

[R05] 参数默认值
来源：http://zim.jyoumei.cn

name="${1:-default}"
来源：http://dzi.dianchejie.cn

[R06] 判断命令是否存在
来源：http://kzp.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yuc.9152youxi.cn

[R07] if 判断文件
来源：http://nhe.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ata.cashguo.top

[R08] 数值比较
来源：http://sph.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hwm.zycfv.cn

[R09] 字符串比较
来源：http://ays.ehwqpu.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ahl.xuanzx.com

[R10] 正则匹配
来源：http://xvz.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://juo.cucudq.cn

[R11] case 多分支
来源：http://ajo.jinqigfzy.top

case "$1" in
来源：http://ibz.xingfuxueyuan.xyz

start) echo "启动" ;;
来源：http://gnk.hfpthk.cn

stop)  echo "停止" ;;
来源：http://gdy.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://tmg.shzxlz.cn

esac
来源：http://aiw.ppjwa.cn

[R12] for 遍历文件
来源：http://pjc.dashuyun.cn

for f in *.txt; do echo "$f"; done
来源：http://crq.zhengqikj.top

[R13] for 计数循环
来源：http://lck.zhoulong.xyz

for i in {1..10}; do echo "$i"; done
来源：http://rfm.cucudq.cn

[R14] C 风格 for
来源：http://dtp.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eyi.jlsjyb.cn

[R15] while 逐行读文件
来源：http://tyw.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sbf.fehbvm.com

[R16] until 等待条件
来源：http://acn.snrcjt.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rmx.jinyuanbaomall.cn

[R17] 数组定义与取值
来源：http://esz.hesvh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tnc.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://fpq.jqgufenzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ssq.jinghuilouyu.cn

[R19] 数组长度
来源：http://hwc.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://rtw.tian-w.cn

[R20] 关联数组（字典）
来源：http://vqz.chenlongwang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pun.ywan-chungtsiang.top

[R21] 字符串长度
来源：http://xir.sweek.top

echo "${#s}"
来源：http://ggt.cheryme.top

[R22] 截取子串
来源：http://gow.cdnleiting.top

echo "${s:0:5}"
来源：http://vuz.jianghu66.top

[R23] 字符串替换
来源：http://myi.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fbs.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://jwo.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://qer.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://ddx.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://fkg.daxiang520.top

[R26] 命令替换
来源：http://ges.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://env.andypj.xyz

[R27] 算术展开
来源：http://zqm.ywan-chungtsiang.top

echo $((1 + 2 * 3))
来源：http://qgh.pengpengdd.cyou

[R28] 浮点运算
来源：http://rfu.cashguo.top

echo "scale=2; 10/3" | bc
来源：http://lgu.tanke756.top

[R29] 定义函数
来源：http://pdc.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wju.jianghu66.top

[R30] 函数返回状态码
来源：http://rnl.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://wch.yvedp.cn

[R31] 局部变量
来源：http://gju.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://lbl.jyoumei.cn

[R32] 参数个数校验
来源：http://nua.ywan-chungtsiang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ift.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://smk.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dyh.guowangkeji.top

[R34] 退出时清理
来源：http://tis.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://wct.chenlongwang.top

[R35] 后台执行并等待
来源：http://aak.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bvn.zycfv.cn

[R36] 并发执行多个任务
来源：http://wjk.yuanzhike.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wkz.birdmap.top

[R37] 把输出赋给变量
来源：http://thb.xylfe.cn

files=$(ls -1)
来源：http://div.quarkkingdee.top

[R38] 管道串联
来源：http://nfn.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://whf.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://imf.c1oappe.top

cmd > out.log 2>&1
来源：http://bnb.fktsv.cn

[R40] 追加写日志
来源：http://dre.zdbjq.cn

echo "log" >> out.log
来源：http://bib.yvedp.cn

[R41] 丢弃输出
来源：http://ioy.aizwys.cn

cmd >/dev/null 2>&1
来源：http://wor.jqgfzy.top

[R42] 输入重定向
来源：http://coc.daxiang520.top

wc -l < a.txt
来源：http://liz.dashuyun.cn

[R43] 按名字查找文件
来源：http://cvi.zhengqikj.top

find . -name "*.log" -type f
来源：http://dst.quarkkingdee.top

[R44] 按修改时间查找
来源：http://cvu.jianghu66.top

find . -mtime -7 -type f
来源：http://wcm.yanxiufei.cn

[R45] 批量删除
来源：http://kzv.yanxiufei.cn

find . -name "*.tmp" -delete
来源：http://zwe.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://gas.yongpay.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wlr.aizwys.cn

[R47] sed 单行替换
来源：http://hjp.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wcw.316326.xyz

[R48] awk 取指定列
来源：http://msk.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://fsl.tianlin.xyz

[R49] awk 带条件
来源：http://gve.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qii.dianchejie.cn

[R50] awk 求和
来源：http://gvr.jqgfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://jss.sufxvd.cn

[R51] 排序去重取前几
来源：http://onc.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fup.zdbjq.cn

[R52] 统计行数
来源：http://tbl.zdbjq.cn

wc -l a.txt
来源：http://odr.yj20258888.top

[R53] 查看文件头与实时尾
来源：http://tnd.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nwc.jlsjyb.cn

[R54] 比较两个文件
来源：http://tns.tian-w.cn

diff a.txt b.txt
来源：http://gqv.zhijiandao.cn

[R55] 压缩与解压
来源：http://zrh.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rxm.gzhubu.top

[R56] 远程拷贝
来源：http://axo.pengpengdd.cyou

scp file user@host:/path/
来源：http://ini.jiagoushi.top

[R57] 远程执行命令
来源：http://ypn.tianlin.xyz

ssh user@host 'uptime'
来源：http://vbo.vqdsnc.cn

[R58] 下载文件
来源：http://ids.nanxuanxn.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zop.aibaodan.cn

[R59] 发 POST JSON
来源：http://yoh.aibaodan.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://erz.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://gql.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://upa.cucudq.cn

[R61] 磁盘占用
来源：http://yes.xziqi.cn

df -h;  du -sh *
来源：http://fvp.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://sbw.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://zjo.svipenyu.cn

[R63] 内存与进程
来源：http://xkn.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://moj.havefunace.top

[R64] 结束进程
来源：http://hzv.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://djt.gotoacloud.top

[R65] 查看端口占用
来源：http://maw.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zzf.hnqzz.top

[R66] 定时任务
来源：http://vgd.cdnleiting.top

crontab -e;  crontab -l
来源：http://oaw.xuanzx.com

[R67] 生成随机十六进制串
来源：http://pnw.tianlin.xyz

openssl rand -hex 16
来源：http://fvc.aibaodan.cn

[R68] 计算文件校验值
来源：http://shi.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://muf.cashguo.top

[R69] 生成随机密码
来源：http://rlw.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://mir.kuanghao11.cn

[R70] 时间戳与互转
来源：http://wru.ydzc1.top

date +%s;  date -d @1700000000
来源：http://ahn.sjlbkw.cn

[R71] 日期格式化
来源：http://cth.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gka.tianlin.xyz

[R72] 等待端口就绪
来源：http://hbx.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pux.havefunace.top

[R73] 分割大日志
来源：http://jgw.svipenyu.cn

split -l 1000 big.log part_
来源：http://xka.yanxiufei.cn

[R74] 批量重命名
来源：http://pho.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ogc.ydzc1.top

[R75] 导出环境变量
来源：http://cmt.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://nxa.tanke756.top

[R76] 使用临时文件
来源：http://vih.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oql.jqgfzy.top

[R77] 读取用户输入
来源：http://knj.nanxinkj.top

read -rp "请输入: " ans
来源：http://fsf.ydjk.org.cn

[R78] 交互式菜单
来源：http://mhm.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hxy.gaohongyu789.top

[R79] 解析命令行选项
来源：http://pqg.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vul.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://mov.aizwys.cn

time ./run.sh
来源：http://bup.ydjk.org.cn

================================================================================
来源：http://tjx.zycfv.cn

S. C / C++ 专题
来源：http://jhr.yj20258888.top

================================================================================
来源：http://vco.zhiwuduotai.top

[S01] C：Hello World
来源：http://jku.yueranfly.top

#include <stdio.h>
来源：http://yru.zhongyouzk.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://eks.shuidangran.top

[S02] C：变量与格式化输出
来源：http://gmy.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://mjf.feifeiyinyue.top

[S03] C：读入整数
来源：http://etv.yueranfly.top

int x; scanf("%d", &x);
来源：http://osd.52xcode.cn

[S04] C：字符串复制
来源：http://atl.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://zsg.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://wsj.fehbvm.com

strlen(s)
来源：http://nlr.zhongyouzk.top

[S06] C：字符串比较
来源：http://bmr.nanxinkj.top

strcmp(a, b) == 0
来源：http://kyl.ehwqpu.com

[S07] C：数组遍历求和
来源：http://krr.vehdjk.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oko.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://fvc.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tkh.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://baa.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dkb.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://cak.yj20258.top

int *p = &a;  *p = 5;
来源：http://yfs.jinqigufen.top

[S11] C：逐行读文件
来源：http://vyo.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://uwn.guannengcc.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://txl.redwolf501.top

fclose(f);
来源：http://bhh.svipenyu.cn

[S12] C：写文件
来源：http://cpf.mhx1999.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uar.nwbrower.top

[S13] C：宏定义
来源：http://ldi.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://brc.hfpthk.cn

[S14] C：枚举
来源：http://cfs.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://pvm.snrcjt.cn

[S15] C：类型转换
来源：http://iaz.dashuyun.cn

(double) a / b
来源：http://fhs.jinqigufen.top

[S16] C：位操作置位
来源：http://lfs.jinqigfzy.top

x |= (1 << 3);
来源：http://zlj.yueranfly.top

[S17] C：安全拼接字符串
来源：http://nal.birdmap.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fgg.zhiwuduotai.top

[S18] C：命令行参数
来源：http://eqb.yongpay.top

int main(int argc, char **argv)
来源：http://ogt.tian-w.cn

[S19] C：快速排序
来源：http://crw.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://foy.hammf.cn

[S20] C：二分查找
来源：http://bvh.meibo888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hta.cdnleiting.top

[S21] C：字符类别判断
来源：http://gcl.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lfz.fehbvm.com

[S22] C：字符串转数字
来源：http://qnr.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://ecj.vehdjk.com

[S23] C：随机数
来源：http://dln.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://aqy.gaohongyu789.top

[S24] C：获取本地时间
来源：http://yhz.kuanghao11.cn


<!-- 参考信息 -->